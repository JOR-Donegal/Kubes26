# Architecture

K8s is a combination of tools, concepts and architecture.

## Pod
In K8s, a _pod_ is the smallest entity we consider, it may just hold a single container, or multiple containers. 

## Worker Node
A pod runs on a _worker node_. I might stand up a Ubuntu server to act as a worker node. I may run many pods on a worker node. As a starting point, you need to create at least one worker node. You may need multiple worker nodes for an application.

## Proxy
K8s sets up a _proxy_ on each worker node to control networking to the pods.

## Master Node
You do not control anything via worker nodes. The _control plane_ of K8s works via a _master node_. On a simple system with one worker node, you may colocate the master node. 

## Cluster
An assemblage with a master node and worker node(s) is a K8s _cluster_.