#### Uses the pre-configured OpenShift cluster
oc login
#### Allows you to log in to any OpenShift cluster
oc login cluster address
#### Log out
oc logout
#### See current project
oc project
#### Create a new project
oc new-project <project name>
#### List all projects
oc projects
#### Switch projects
oc project <project name>
#### Get built-in documentation for Pods
oc explain pod
#### Get details on the pod's spec
oc explain pod.spec
#### Get details on the pod's containers
oc explain pod.spec.containers
#### Creating Pods from files
#### Create a Pod on OpenShift based on a file
oc create -f pods/pod.yaml
#### Show all currently running Pods
oc get pods
#### Port forwarding for Pods
#### Open a local port that forwards traffic to a pod
oc port-forward <pod name> <local port>:<pod port>
#### Example of 8080 to 8080 for hello world
oc port-forward hello-world-pod 8080:8080
#### Get built-in documentation for Pods
oc explain pod
#### Get details on the pod's spec
oc explain pod.spec
#### Get details on the pod's containers
oc explain pod.spec.containers
#### You can use this oc explain command to get info about any of the other fields in a Pod
#### oc rsh will work with any Pod name 
oc rsh <pod name>
#### Check the API on port 8080
wget localhost:8080
#### Exit the rsh session
exit

