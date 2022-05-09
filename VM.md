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

* Can you list some VM technologies and explain their use?

**VirtualBox**

VirtualBox is a free and open-source hypervisor for x86 computers that is developed by Oracle.  It can be installed on a number of host operating systems, such as Linux, macOS, Windows, Solaris and OpenSolaris.

**Windows Virtual PC**

Windows Virtual PC is a freeware virtualisation program designed for Microsoft Windows. It does not run on versions earlier than Windows 7 and does not support MS-DOS or operating systems earlier than Windows XP Professional SP3.

**Kernel-based Virtual Machine**

A Kernel-based Virtualisation Machine is a virtualisation infrastructure for Linux kernel which develops into a hypervisor.

KVM originally supported x86 processors and an ARM port, before being merged during the 3.9 kernel merge window.

**Hyper-V**

Hyper-V, formerly named Windows Server Virtualisation, is a hypervisor designed to create virtual machines on x86-64 systems running Windows.

A server computer that runs Hyper-V can be configured to expose individual virtual machines to one or more networks.

Hyper-V carries out the isolation of virtual machines in terms of a partition, a logical unit of isolation that is supported by the hypervisor that each operating system executes in.

The Hyper-V does not virtualise audio hardware, and does not require users to have an existing installation of Windows Server 2008 or R2.

The Hyper-V Server is built with components of Windows with an included Windows Server Core user experience.

**VMware Workstation Player**

VMware Workstation Player is virtualisation software packaged for x64 computers running Microsoft Windows or Linux that is offered free of charge by VMware.

VMware workstation playerIts VMware Player is able to run all existing virtual appliances and also create its own virtual machines, using the same virtualisation core as VMware Workstation.

![VM](https://user-images.githubusercontent.com/103209557/167372361-1a26e14d-9f9f-4eca-953f-6ffe88f44ce3.jpg)
