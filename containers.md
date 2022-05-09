**What is a container?**

Containers are lightweight software packages that contain all the dependencies required to execute the contained software application. These dependencies include things like system libraries, external third-party code packages, and other operating system level applications. The dependencies included in a container exist in stack levels that are higher than the operating system.

*Pros*

* Iteration speed

* Because containers are lightweight and only include high level software, they are very fast to modify and iterate on.

* Robust ecosystem

* Most container runtime systems offer a hosted public repository of pre-made containers. These container repositories contain many popular software applications like databases or messaging systems and can be instantly downloaded and executed, saving time for development teams

*Cons*

* Shared host exploits

* Containers all share the same underlying hardware system below the operating system layer, it is possible that an exploit in one container could break out of the container and affect the shared hardware. Most popular container runtimes have public repositories of pre-built containers. There is a security risk in using one of these public images as they may contain exploits or may be vulnerable to being hijacked by nefarious actors.

![containers](https://user-images.githubusercontent.com/103209557/167378765-45330b82-c3f5-481b-b57a-0de27830ff33.png)

## Different types of container

There are two types of container in general.They are application container and system container.


### OS(system) containers

OS containers are virtual environments that share the kernel of the host operating system but provide user space isolation. For all practical purposes, you can think of OS containers as VMs. You can install, configure and run different applications, libraries, etc., just as you would on any OS. Just as a VM, anything running inside a container can only see resources that have been assigned to that container.

OS containers are useful when you want to run a fleet of identical or different flavors of distros. Most of the times containers are created from templates or images that determine the structure and contents of the container. It thus allows you to create containers that have identical environments with the same package versions and configurations across all containers.



### Application containers

While OS containers are designed to run multiple processes and services, application containers are designed to package and run a single service. Container technologies like Docker and Rocket are examples of application containers. So even though they share the same kernel of the host there are subtle differences make them different, which I would like to talk about using the example of a Docker container:

Run a single service as a container

When a Docker container is launched, it runs a single process. This process is usually the one that runs your application when you create containers per application. This very different from the traditional OS containers where you have multiple services running on the same OS.

Any RUN commands you specify in the Dockerfile creates a new layer for the container. In the end when you run your container, Docker combines these layers and runs your containers. Layering helps Docker to reduce duplication and increases the re-use. This is very helpful when you want to create different containers for your components. You can start with a base image that is common for all the components and then just add layers that are specific to your component. Layering also helps when you want to rollback your changes as you can simply switch to the old layers, and there is almost no overhead involved in doing so.

![os-vs-app-containers](https://user-images.githubusercontent.com/103209557/167381527-efabc0e8-ac36-4c4e-aaf9-ad312a774a89.jpeg)


Within the platform, different container types can be used for various use cases:

Certified Managed Containers.

Elastic Virtual Private Servers (Elastic VPS)

Custom Docker Containers.

Docker Engine CE (Docker Native)

Kubernetes Cluster.

