 # VIRTUALIZATION 
                                          
### Types of virtualization   
       
 **Hardware virtualization:** When virtualizing hardware, virtual versions of computers and operating systems (VMs) are created and consolidated into a single, primary, physical server.
 **Software virtualization:** Software virtualization creates a computer system complete with hardware that allows one or more guest operating systems to run on a physical host machine.
 **Storage virtualization:** Storage can be virtualized by consolidating multiple physical storage devices to appear as a single storage device. Benefits include increased performance and speed, load balancing and reduced costs.
 **Network virtualization:** Multiple sub-networks can be created on the same physical network by combining equipment into a single, software-based virtual network resource. Network virtualization also divides available bandwidth into multiple, independent channels, each of which can be assigned to servers and devices in real time.
 **Desktop virtualization:** This common type of virtualization separates the desktop environment from the physical device and stores a desktop on a remote server, allowing users to access their desktops from anywhere on any device.
                                                            
 ###   VIRTUAL MACHINES(VM) 
 A virtual machine is the emulated equivalent of a computer system that runs on top of another system. Virtual machines may have access to any number of resources: computing power, through hardware-assisted but limited access to the host machine's CPU and memory; one or more physical or virtual disk devices for storage; a virtual or real network inferface; as well as any devices such as video cards, USB devices, or other hardware that are shared with the virtual machine.   
***NB***: Each virtual machine runs its own operating system and functions separately from the other VMs, even when they are all running on the same host. 
USES:
*Virtual machines (VMs) allow a business to run an operating system that behaves like a completely separate computer in an app window on a desktop.
*VMs may be deployed to accommodate different levels of processing power needs, to run software that requires a different operating system, or to test applications in a safe, sandboxed environment. etc...

 #### Types of virtual machine   
 1. A process virtual machine allows a single process to run as an application on a host machine, providing a platform-independent programming environment by masking the information of the underlying hardware or operating system
 2. A system virtual machine is fully virtualized to substitute for a physical machine. A system platform supports the sharing of a host computer’s physical resources between multiple virtual machines, each running its own copy of the operating system. This virtualization process relies on a hypervisor, which can run on bare hardware, such as VMware ESXi, or on top of an operating system.
                                          
 ### LINUX CGROUPS AND NAMESPACES
 CGROUPS: Cgroups, which stands for control groups, are a kernel mechanism for limiting and measuring the total resources used by a group of processes running on a system. For example, you can apply CPU, memory, network or IO quotas.                                                                   
 NAMESPACES: Namespaces are a kernel mechanism for limiting the visibility that a group of processes has of the rest of a system. For example you can limit visibility to certain process trees, network interfaces, user IDs or filesystem mounts.                                                                    
 ###  APPLICATIONS CONTAINERS 
Application containers are used to package applications without launching a virtual machine for each app or each service within an app. They are especially beneficial when making the move to a microservices architecture, as they allow you to create a separate container for each application component and provide greater control, security and process restriction. Ultimately, what you get from application containers is easier distribution. The risks of inconsistency, unreliability and compatibility issues are reduced significantly if an application is placed and shipped inside a container. Application containers are the primary use case for Docker.
       
### VAGRANT                      
 This is a tool for working with virtual machines. Vagrant is a tool for working with virtual environments, and in most circumstances, this means working with virtual machines. Vagrant provides a simple and easy to use command-line client for managing these environments, and an interpreter for the text-based definitions of what each environment looks like, called Vagrantfiles.                                                                 
 The difference between vagrant and other virtual machines hypervisoris; vagrant adds an additional layer is simplicity, interoperability across multiple systems, and a more consistent approach which could theoretically be used with any virtual environment running on top of any other system.
                          
### H Y P E R V I S O R
 A hypervisor is a program for creating and running virtual machines. There are traditionally two classes:
i. Bare metal hypervisor: This runs guest virtual machines directly on a system's hardware, essentially behaving as an operating system.
ii. Hosted hypervisor : This behaves more like traditional applications that can be started and stopped like a normal program.                                                                                         
 ### DOCKER
 The term "docker" may refer to either the tools (the commands and a daemon) or to the Dockerfile file format.
  Docker is a software framework for building, running, and managing containers on servers and the cloud. The Docker engine can be useful for lone developers who need a lightweight, clean environment for testing, but without a need for complex orchestration.                               
### PROXMOX
 It is a Debian-based Linux distribution that allows and allows deployment and management of virtual machines and containers. Proxmox employs kernel virtual machine (KVM) virtualization to support just about any operating system that you can download and install into a fully virtualized collection of hardware. 
### PODMAN
 Podman is a daemonless container engine for developing, managing, and running OCI Containers on your Linux System. Containers can either be run as root or in rootless mode. This can be used an a replacement for Docker and m	ost Docker commands can be directly translated to Podman commands. 
### SYSTEM CONTAINERS
 It is a stateful, operating system-centric solution that can run multiple processes. System containers are usually used for traditional or monolithic applications, as they allow to host architectures, tools, and configurations implemented for VMs. There are different implementations of system containers: LXC/LXD, OpenVZ/Virtuozzo, BSD jails, Linux vServer, and some others. 
### LXC
 LXC is a well-known Linux container runtime that consists of tools, templates, and library and language bindings. It's pretty low level, very flexible and covers just about every containment feature supported by the upstream kernel. LXC provides the basic functionality used under the hood by LXD.  
### KUBERNETS
 Kubernetes is an open-source container orchestration platform that enables the operation of an elastic web server framework for cloud applications. Kubernetes can support data center outsourcing to public cloud service providers or can be used for web hosting at scale. Website and mobile applications with complex custom code can deploy using Kubernetes on commodity hardware to lower the costs on web server provisioning with public cloud hosts and to optimize software development processes.
 
  Kubernetes features the ability to automate web server provisioning according to the level of web traffic in production. Web server hardware can be located in different data centers, on different hardware, or through different hosting providers. Kubernetes scales up web servers according to the demand for the software applications, then degrades web server instances during downtimes. Kubernetes also has advanced load balancing capabilities for web traffic routing to web servers in operations.
### ESXi
 This is a type 1 hypervisor from VMware. VMware ESXi effectively partitions hardware to consolidate applications and cut costs. 
 *ESXi enables you to: 

    Consolidate hardware for higher capacity utilization.
    Increase performance for a competitive edge.
    Streamline IT administration through centralized management.
    Reduce CapEx and OpEx.
    Minimize hardware resources needed to run the hypervisor, meaning greater efficiency.
    
**FEATURES:**
i. By consolidating multiple servers onto fewer physical devices, ESXi reduces space, power and IT administrative requirements while driving high-speed performance.
ii. Small Footprint
iii. With a footprint of just 150MB, ESXi lets you do more with less while minimizing security threats to your hypervisor.
iv.Reliable Performance
v. Accommodate apps of any size. Configure virtual machines up to 128 virtual CPUs, 6 TB of RAM and 120 devices to satisfy all your application needs. Consult individual solution limits to ensure you do not exceed supported configurations for your environment. Learn more about configuration maximums.
vi. Enhanced Security
vii. Protect sensitive virtual machine data with powerful encryption capabilities. Role-based access simplifies administration, and extensive logging and auditing ensure greater accountability and easier forensic analysis.
viii. Ecosystem Excellence
ix. Get support for a broad ecosystem of hardware OEM vendors, technology service partners, apps, and guest operating systems.
x. User-Friendly Experience
xi. Manage day-to-day administrative operations with built-in modern UI based on HTML5 standards. For customers who need to automate their operations, VMware offers both a vSphere Command Line Interface and developer-friendly REST-based APIs.

                     
   >THE USE OF VM's MAKES LIFE EASIER IN THE IT WORLD AND HS MORE ADVANTAGES, SO I THINK IT'S ADVANTAGEOUS AND WORTH INVESTING INTO.