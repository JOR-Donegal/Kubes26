# Introduction

!!! abstract "Kubernetes (K8s)"

Before beginning these notes, ensure you have completed my notes and exercises on Docker.

In my exercises on _Docker_, we saw how to create and deploy containers; _orchestration_. Docker-Compose is appropriate for doing development on a single host.

In a production environment, this may need to be done at scale.
_Kubernetes_ (K8s) allows us to deploy, scale and manage across multiple hosts:

K8s lets us

- Deploy containers in an automated manner
- Monitor their state
- Take management actions if they crash or go down or need replacement
- Scale up containers, create more instances to cope with load, and the converse
- Load balancing across multiple instances
- Manage networking and storage

_Docker-Compose_ allowed us to manage multi-container projects. K8s could be considered as an orchestration system across multiple machines.   

Services like _AWS ECS_ may be useful in some of these areas, but it takes some control away from us. Vendor Lock-in!  K8s is _open source_ and gives us orchestration independent of platform. It allows us to script to any cloud provider or to our own servers in private cloud. Rewriting this in 2026, _sovereignty_ has become a critical concern.

A K8s configuration file is a standardized example of infrastructure as code.

As always, consider my notes a summary and a starting point. Definitive information may be found at the [Kubernetes](https://kubernetes.io/) web site.

