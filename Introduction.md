
### Basic Introduction

* Back to history in 2001 linux introduces a project name VServer
* It was first attempt for running complete set of processes inside one server with high degree isolation
* Features of linux in containers :
* [Namespaces]
     1. By placing resources in namespaces only the processes which is the member of namespaces can able to see it
     
* [Control groups]
    1. It partitions process and their children into groups to limit them from using specific resources they are assigned only some resources which they have to use 
* [Secomp]
    1. It defines the security profile of processes
* [Selinux]
    1. Its about protecting containers from each other
    2. Also protecting containers from host machine
    3. By making sure that processes can only interact with the resources which assigned to their user only 
* This is all about to design container!for it  you need to have 
    1. Container as small as possible 
    2. But they need to have everything 
    3. And should spin faster
* Idea to use container is take your big application breks them in small pieces called micro-services and all these micro services will run in separate containers
* So if somethings got brek it wont effect to other container or service or functionality 
* We need to reuse of container we don't want to do same process to deploy container in order to do it here comes the container image
* Docker Image:
    1. A file system bundle that contains all dependencies related to execute a process
    2. Image will have everything you need to create a container
    3. From image we can create as many containers e want and we can scale them up to handle multiple request 