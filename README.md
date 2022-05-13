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

