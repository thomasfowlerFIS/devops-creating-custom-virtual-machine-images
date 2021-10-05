# **Creating Custom Virtual Machine Images**

Course: DevOps

Mod: Week 1

Topic: Creating Custom Virtual Machine Images

Amount of time: 1.5 hours

Author: Thomas Fowler

--------------------------------------------

## **Lesson Objectives**

* Describe the steps necessary to create a virtual machine image.

* List the two file types associated with virtual machine images
or virtual appliances.

* Understand the various levels of configuration for a virtual machine image.

--------------------------------------------

### **Overview**

<!-- talk about the reason and benefits behind custom vm images -->
Creating custom virtual machine images or virtual appliances is beneficial
for many reasons. The primary reason is the ability to provide turn-key
solutions for the technology organization that fit a variety of use cases.

Take for example, an application development team that needs a compute
instance with the ability to run a Java Spring Boot or Go application
with all the necessary dependencies and configuration. Such an instance
can be pre-configured and provisioned, tested, and certified before ever
reaching the application development team. This means, by the time the
compute instance or virtual appliance is ready, the application development
team merely needs to deploy its application, without any additional
configuration or software dependency installation.

Additionally, virtual appliances are portable across different hypervisors
from various vendors, allowing for even greater flexibility for when and
how compute instances are provisioned and deployed.

--------------------------------------------

### **Creating a Virtual Machine Image**

When creating a custom virtual machine or virtual appliance, there are two
format choices in VirtualBox from which the user may select. The first and
most common is OVF or Open Virtualization Format.

OVF may come as one file or several files depending on the exporter's
selections during the export process. OVF also includes a companion manifest
file in XML format that provides necessary information for VirtualBox and
other hypervisors to import the VMDK (an open virtual disk image format)
properly.

The other option for creating a virtual appliance is using the OVA or Open
Virtual Archive format which is a variation of the TAR archive format. OVA
archives can be opened outside of the VirtualBox which is appealing for
systems administrators managing other hypervisor solutions.

--------------------------------------------

### **Virtual Appliance Import and Export**

The following sections describe the process by which to export and import
virtual applicances, respectviely. Certain options for both importing and
exporting will produce different results based on the options chosen. 

**_Note_**: It is important to pay particular attention to the options for
import and export, as they may have unintended side effects on a system if
the incorrect options are chosen.

#### **Exporting a Virtual Appliance**

<img src="https://raw.githubusercontent.com/thomasfowlerFIS/devops-creating-custom-virtual-machine-images/assets/exportingVM_Step1.png" width="500" />

#### **Importing a Virtual Appliance**

--------------------------------------------

### **Additional Configuration**

<!-- discuss add'l config options for further customization -->
