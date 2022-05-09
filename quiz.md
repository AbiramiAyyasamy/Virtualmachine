## What Are Virtual Machines (VMs)?

 Historically, as server processing power and capacity increased, bare metal applications weren’t able to exploit the new abundance in resources. Thus, VMs were born, designed by running software on top of physical servers to emulate a particular hardware system. A hypervisor, or a virtual machine monitor, is software, firmware, or hardware that creates and runs VMs. It’s what sits between the hardware and the virtual machine and is necessary to virtualize the server.

Within each virtual machine runs a unique guest operating system. VMs with different operating systems can run on the same physical server—a UNIX VM can sit alongside a Linux VM, and so on. Each VM has its own binaries, libraries, and applications that it services, and the VM may be many gigabytes in size.

Development also benefited from this physical consolidation because greater utilization on larger, faster servers freed up subsequently unused servers to be repurposed for QA, development, or lab gear.   But this approach has had its drawbacks. Each VM includes a separate operating system image, which adds overhead in memory and storage footprint.

 As it turns out, this issue adds complexity to all stages of a software development lifecycle—from development and test to production and disaster recovery. This approach also severely limits the portability of applications between public clouds, private clouds, and traditional data centers.
 
  ## What Are Containers? 
 
 Docker is a tool that uses containers to make creation, deployment, and running of application a lot easier. It binds application and its dependencies inside a container.
 
 Operating system (OS) virtualization has grown in popularity over the last decade to enable software to run predictably and well when moved from one server environment to another. But containers provide a way to run these isolated systems on a single server or host OS.


**What are the differences between system containers, application containers and virtual machines?**

In Docker, the containers running share the host OS kernel. A Virtual Machine, on the other hand, is not based on container technology. They are made up of user space plus kernel space of an operating system. Under VMs, server hardware is virtualized.

Docker is a container-based technology that lets you develop distributed applications. I will explain the differences between virtual machines and Docker containers.

### Docker(Container)
* Containers are destroyed and re-created rather than moving
* OS level process isolation
* Boots in seconds
* Less resource usage	
* Pre-built docker containers are easily available

### Virtual Machine

* VMs can move to new host easily	Containers are destroyed and re-created rather than moving
* Hardware-level process isolation	
* Boots in minutes	
* More resource usage	
* Ready-made VMs are difficult to find.

![containers-vs-virtual-machines](https://user-images.githubusercontent.com/103209557/167423739-f5b140ad-990a-47e1-a802-6a65692a9246.jpg)

**In your opinion, when does it make sense to use either a virtual machine, a system container or an application container?**
When should you use a Docker container or a virtual machine?

In my opinion, when does it make sense to use either a virtual machine, a system container or an application container?

The docker containers are suited for situations where you want to run multiple applications over a single operating system kernel.

But if you have applications or servers that need to run on different operating system flavors, then virtual machines are required.

![vmordocker](https://user-images.githubusercontent.com/103209557/167424957-8a28661b-e42e-4f52-8046-ccc93030c4b1.png)
