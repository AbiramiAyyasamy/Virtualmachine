## Container runtimes
Docker was the first major open-source container offering, and quickly emerged as a de facto standard. Now Kubernetes is evolving as the new standard for clusters and cluster management.

* Docker
The first and still most popular container technology, Docker's open-source containerization engine works with most of the products that follow, as well as many open-source tools.

* Docker Enterprise
This set of extensions not only adds features to Docker, but also makes it possible for Docker (the company) to add commercial support. If you need a support matrix to know exactly which versions of what software are supported—and a phone number to call if things go wrong—then Docker Enterprise might be for you.

* CRI-O
The first implementation of the Container Runtime Interface, CRI-O is an incredibly lightweight, open-source reference implementation.

## Cluster management and deployment

Once the team can create images and pass them around in development, comes the hard part: running and supporting containers in production. That means registering artifacts, deploying them to production as a system, and managing servers and collections of servers. The latter includes a collection of servers in the cloud, known as a "cluster." 

## Examples

* Kubernetes

While there is no standard for cluster management, the Kubernetes open-source cluster manager, originally developed by Google, is far and away the most popular. Supported by Amazon's AWS, Google's Cloud Engine (GCE) and Microsoft's Azure Container service, Kubernetes is relatively portable, which helps prevent vendor lock-in.

Kubernetes can even run on a private cloud: OpenStack. Microsoft, Amazon, and Google all provide container services that run Kubernetes—with commercial support options available.

* Istio and Envoy

Envoy and Istio are open-source service mesh technologies that add a layer to provide security and observability. They can encrypt traffic inside of the cluster while observing it. Developed by Lyft, Envoy was the first service mesh for Kubernetes. Istio includes Envoy, sits on top of it, and adds several plugins, dashboards, and other features to extend it. 


### Storage containers

Containers are designed to be interchangeable, like currency. That works exceptionally well for web services and microservices that can scale on demand. Storage and databases, on the other hand, need persistent locations to house data, or at least a standard interface layer. Organizations that want to move to an all-container infrastructure need storage, and companies now meet that demand.

* BlockBridge
BlockBridge, the "elastic storage platform" company, offers storage as a container using Docker, with support for Kubernetes, OpenStack, and software-defined secure storage.

* EMC / libstorage
The EMC / libstorage system offers a code library to provide container storage that's free and open.

* Docker plugins for storage
EMC, NetApp, and others have created plugins to support storage, which Docker Inc. makes available for download.

## Operating systems 

Most Linux operating system distributions are based on convenience and include big, preinstalled packages, just in case the user might want them. Docker, in contrast, is designed for lightweight virtualization—to run as many identical machines as possible with the least amount of overhead in terms of memory, disk, and CPU.

* RancherOS

Containing only the Linux kernel and Docker itself, the RancherOS system image fits into just 22MB of disk space. RancherOS eliminates systemd, the service management system built into most versions of Linux, instead starting the Docker Daemon itself as the init, or bootstrap, system.

* CoreOS Container Linux

Designed to work with CoreOS Linux tools and systems, CoreOS Container Linux is preconfigured to run Linux containers. It also comes with automatic updates turned on; operating systems update themselves without any handling.

* Ubuntu Core

Canonical, the parent company of Ubuntu Linux, claims that Ubuntu is the most common OS for containers. Within the Ubuntu distribution is Core, the small, secure release designed for Internet of Things devices and containers. Core is designed to have high performance, a small footprint, and transactional updates, ensuring that updates that fail roll back successfully. Of course, using Ubuntu Core means you can purchase support from Canonical.

* Red Hat Atomic Host

Organizations that run Red Hat Enterprise and want to use containers will want to have their hosts run the Red Hat Atomic Host operating system. These tools will let you host Linux containers in a minimal version of Red Hat Enterprise Linux.

## Why are containers so inherently linked to Linux?

Ultimately, containers are a feature of Linux. Containers have been a part of the Linux operating system for more than a decade, and go back even further in UNIX. That's why, despite the very recent introduction of Windows containers, the majority of containers we see are in fact Linux containers.

* Does Kubernetes use Docker?

Kubernetes is removing support for Docker as a container runtime. Kubernetes does not actually handle the process of running containers on a machine. Instead, it relies on another piece of software called a container runtime.

* Is Docker the future?

Docker has been tipped as the future of virtualisation. Its popularity is definitely growing, especially with companies like Netflix, Spotify, PayPal and Uber using the containerisation system. Hyve provides hosting for Docker containers on our Private Docker platform.
