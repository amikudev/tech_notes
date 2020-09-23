* node
    * A node is a worker machine in k8s. It may be a VM or a physical machine.
    depending on the cluster. Each node contains the services required to run pods and is managed by the master components
    
* deployment
* pod
* service
    * is like a load balancer
* connect to pods/deployments
    * port forwarding
        * kubectl port-forward <pod-name> port-outside:port-in-cluster
        * kubectl port-forward <pod-name> 8081:3000
    * expose a service
        * kubectl expose pod <podname> --type=NodePort --name=<service-name>
        * minikube service <service-name> --url
* The data in a pod is finished as soon as it is finished. If your want persistence, use volumesn
*  

    