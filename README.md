                                       # Kubernetes-Project

# Root level properties in manifest files
1) apiVersion -- kubernetes apiversion used -- v1
2) kind -- what kind of object to create
3) metadata -- data to identify object 
4) spec -- specifications of object.

--> Pod ---------> Replicaset ---------> Deployment 
- Pods controlled and manipulated by replicasets and replicasets manipulated by the deployment.
- Pods should not be adopted directly. with deployment, Pods can be adopted.


# Services --> To expose the pods to network.
 