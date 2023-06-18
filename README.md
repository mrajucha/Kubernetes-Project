                                       # Kubernetes-Project
# GitOps allows teams within an organization to manage and deploy changes to infrastructure using Git as the single source of truth. DevOps, on the other hand, focuses on effectively connecting development and operational teams using a tool of the organization's choosing

# Root level properties in manifest files
1) apiVersion -- kubernetes apiversion used -- v1
2) kind -- what kind of object to create
3) metadata -- data to identify object 
4) spec -- specifications of object.

--> Pod ---------> Replicaset ---------> Deployment 
- Pods controlled and manipulated by replicasets and replicasets manipulated by the deployment.
- Pods should not be adopted directly. with deployment, Pods can be adopted.


# Services --> To expose the pods to network.
- ->  types of services 
- 1) clusterIp(default): create set of ip addresses to cummunicate internal(in node--> db pod to app pod)
                        accessible within the cluster.
- 2) nodePort: expose the each node Ip on static port(nodePort) to access the pod within Node. To make nodePort      
available Kubernetes sets up a cluster IP address, the same as if you had requested a Service of type: ClusterIP.
 
- 3) loadbalancer:





# Helm : kubernetes package manager helps to manage(define,package, install,upgrade) complex kubernetes applications.
- values.yaml --> one file all the configuration(deployment, services, PV's, secrets).
- commands --> helm upgrade
           --> helm list
           --> helm search hub 
           --> helm package 




