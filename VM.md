**What Is a Virtual Machine?**

A virtual machine (VM) is an abstracted instance of a computer system capable of acting like a real, physical computer. Several virtual machines can run separately in parallel on a single underlying device. (You can also virtualize servers, applications, and various other IT components.)


**Why Monitor Virtual Machines?**

Virtual machines need to be managed and monitored for numerous reasons, including:

* Resource management*. First, while virtual machines act as if they’re connected directly to the computer’s hardware, they’re not. There can sometimes be mismatches between what the virtual machine “thinks” it has access to and what the physical hardware can provide. For example, when using thin provisioning, the administrator can make it appear to virtual machines as if they have access to more physical resources than are available on the physical hardware. This can allow virtual machines to function more efficiently, but you can run into problems with slowed performance or crashes when too many virtual machines require resources the hardware can’t provide.

* If one of your virtual machines malfunctions or has been infected with malware, it could start consuming more resources than expected and affect other virtual machines as a result. Monitoring software can detect a rapid change in performance, particularly if one virtual machine quickly starts consuming more resources than it should.

* The configuration of your virtual machines may change at various times, and you need to always ensure configuration changes don’t break or affect something else in your environment in a bad way. With virtualization, the configurations and settings of virtual machines can be easily changed, which means someone can inadvertently change a setting. Monitoring software can alert you to any unexpected changes and can let you know if a change has resulted in performance problems. There are also several processes and operations that can occur in the virtual environment, such as live migration, backups, disaster recovery, or machines powering on and off.

**What is a hypervisor in simple terms?**

A hypervisor, also known as a virtual machine monitor or VMM, is software that creates and runs virtual machines (VMs). A hypervisor allows one host computer to support multiple guest VMs by virtually sharing its resources, such as memory and processing.

The hypervisor manages resources and allocates them to VMs. It also schedules and adjusts how resources are distributed based on how the hypervisor and VMs have been configured, and it can reallocate resources as demands fluctuate. Most hypervisors fall into one of two categories:

Type 1. Also referred to as a bare-metal hypervisor, this type of hypervisor runs directly on the physical host machine and has direct access to its hardware. Type 1 hypervisors typically run on server computers and are considered more efficient and better-performing than Type 2 hypervisors, making them well suited to server, desktop and application virtualization. Examples of Type 1 hypervisors include Microsoft Hyper-V and VMware ESXi.

Type 2. Sometimes called a hosted hypervisor, a Type 2 hypervisor is installed on top of the host machine's OS, which manages calls to the hardware resources. Type 2 hypervisors are generally deployed on end-user systems for specific use cases. For example, a developer might use a Type 2 hypervisor to create a specific environment for building an application, or a data analyst might use it to test an application in an isolated environment. Examples of Type 2 hypervisors include VMware Workstation and Oracle VirtualBox.

**Can you list some VM technologies and explain their use?**
