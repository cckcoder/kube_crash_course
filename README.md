# K8s Crash Course

## K8s Architecture
kub cluster must have atlease 
* one master node
* worker node

## Master node
* API Server
Entrypoint to K8s cluster
  * UI
  * API
  * Cli

* Controller Manager
keeps track of whats happening in the cluster

* Scheduler
ensures Pods placement

* etcd
kube backing storeo

## Worker Node
* higher workload
* much bigger and more resources

## Node (Virtual or physical machine)

### Pod
* Smallest unit in Kube
* Abstraction over container
* Usually 1 Application per Pod
* Each Pod gets its own IP address

### Service
* Permanent IP address
* Lifecycle of Pod and Service not connected

### Deployment
* Blueprint for "my-app" Pods
* you create Deployments
* Abstraction of Pods

### Main kube Components
* Pod => abstraction of containers
* Service => communication
* Ingress => route traffic into cluster
* configMap 
* secret 
* volumn 
* Deployment 
* StatefulSet

## Kube Configuration
* YAML or JSON
* Declarative

### Each Config have 3 part
1 metadata
1 specification
1 status
  * automatic generate by kube

### Minikube and kubectl

#### Cli
* `minikube status`

* `kubectl get node`

* for encrypted
  * `echo -n mongouser | base64`


Kubectl CLI ...for configuring the Minikube cluster

Minikube CLI ...for start up/deleting the cluster

