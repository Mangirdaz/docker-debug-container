Debug Container!
-----------------

From time to time i need to debug something from container. This is sime container containing bunch of defualt tools for what I need".

    $ oc create -f OSE-pod.json

    $ oc get pod hdebug-openshift -o yaml |grep podIP
     podIP: 10.1.0.2

    $ curl 10.1.0.2:8080
     Hello OpenShift!

    $ go build -tags netgo  
    $ mv debug-openshift bin
    $ docker build -t docker.io/mangirdaz/docker-debug-container .
