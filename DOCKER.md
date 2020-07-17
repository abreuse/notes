Docker
====

### Basics

Separates infrastructure from applications.  
Docker helps deploying quickly in production.  

Docker has a daemon which is running in background.  
Command `docker`uses the daemon.  

#### Images

We build images through `Dockerfile` and push images.  
It is fast and convenient, an image on non-prod can be push on production and then be running on a container.  
Rebuilding images with modified `Dockerfile` rebuilds only the layers that have changed.  

#### Registry

Images are stored in the registry. 

#### Containers

Docker works with containers.  
Your running image is called a container.  
It contains everything the image has been built with, database drivers, jvm, plugins, libs.  
This container can be run in non-prod and prod the same way.  

Containers can run on anything (laptop, server, cloud...), it is portable.  

#### Services

Services are used to configure running containers.  
They can set the number of replicas...  
You can enable the `swarm` mode, wich leads to multiple docker daemons communicating through REST API.  
In `swarm` mode, you have `managers` and `workers`.  

### Docker Engine (daemon)

Docker Client communicates to Docker Server through a REST API.  


### Plus

It is great with micro-services environments as it can have multiple containers easily.  
Containers can be managed with `Kubernetes` for even more efficiency.
