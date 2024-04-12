---
layout: post
title: Install Bold BI on GCP Windows instance | Bold BI Docs
description: Discover how to deploy a virtual machine in the Google cloud platform portal and install the Bold BI server application on it.
platform: bold-bi
documentation: ug
---

# Self-deploy a Bold BI Server on Google cloud platform.

Install and run the Bold BI server on an AWS EC2 instance by following these steps.
<ul>
<ol>

1. [Set up a Windows instance on GCP.](https://cloud.google.com/compute/docs/create-windows-server-vm-instance)
2. [Set up a Linux instance on GCP.](https://cloud.google.com/compute/docs/create-linux-vm-instance#:~:text=Create%20a%20Linux%20VM%20instance%201%20In%20the,7%20To%20create%20the%20VM%2C%20click%20Create%20) 

</ol>
</ul>

## Set up a Windows instance on GCP

* Navigate to the Create an instance page in the Google Cloud console.
* Click on Change in the Boot disk section to start configuring your boot disk.
* Select Windows Server from the Operating system list on the Public images tab.
* Select Windows Server 2019 Datacenter from the Version list.
* Click on "Select".
* Under the Firewall section, check the box for "Allow HTTP traffic".
* Click on "Create" to create the VM.
* Wait for a short while for the VM instance to start. Once the VM instance is ready, it will be listed on the VM instances page with a green status icon.

## Connect to Windows Instance
* Navigate to the VM instances page in the Google Cloud console.

* Find your VM instance in the list and click on its name in the "Name" column.

* In the "Remote access" section, click on "Set Windows password".

* Enter a username, then click "Set" to generate a new password for your Windows Server VM. Make sure to save the username and password for logging into the VM.

**Bold BI Installation**

 This section provides instructions on how to install and run the Bold BI server in a virtual machine (VM).

* Features to be enabled in IIS to run Bold BI in Windows Server OS. Refer to this [link](https://help.boldbi.com/faq/features-needed-to-enable-in-iis-to-run-bold-bi-in-win-server-os/).

* Install the Bold BI server on the created Windows virtual machine (VM) in the AWS portal using [help link](https://help.boldbi.com/deploying-bold-bi/deploying-in-windows/)

* Install the Bold BI server on the created Linux virtual machine (VM) in the AWS portal using [help link](https://help.boldbi.com/deploying-bold-bi/deploying-in-linux/installation-and-deployment/#bold-bi-linux-package-installation-and-deployment). 


## Installation steps for Bold BI on an AWS Linux EC2 Instance

### Deploy a Linux Virtual Machine on AWS

* Access the Create an instance page within the Google Cloud console.
* Navigate to the Create an instance screen.
* In the Boot disk segment, select Change to start configuring your boot disk.
* Under the Public images tab, opt for Ubuntu from the Operating system list.
* Select Ubuntu 20.04 LTS from the Version list.
* Choose Select.
* Within the Firewall section, enable Allow HTTP traffic.
* To finalize the creation of the VM, select Create.

## Connect to Windows Instance

* Navigate to the "VM instances" page.
* Locate the VM instance you want to connect to and click on the "SSH" button next to it. This will open a new browser window with an SSH connection to your VM.
* Open a terminal on your local machine.Use the following SSH command to connect to your VM:
    ```bash
        gcloud compute ssh [INSTANCE_NAME] --zone [ZONE]

* Replace [INSTANCE_NAME] with the name of your VM instance and [ZONE] with the zone where your VM is located. You can find this information on the VM instances page in the Google Cloud Console.

* If this is your first time connecting to the VM, SSH will ask you to confirm the connection by typing yes and then enter the password for the user you specified when creating the VM.

* Once connected, you will have a terminal window open that allows you to interact with your Linux VM.


### Installing and running the Bold BI Server on Linux
This section provides instructions on how to install and run the Bold BI server on a Linux virtual machine (VM).
* Install the Bold BI server on the Linux virtual machine (VM) created in the AWS portal using the [help link](https://help.boldbi.com/deploying-bold-bi/deploying-in-linux/installation-and-deployment/bold-bi-on-ubuntu/)
  ![Start up](/static/assets/installation-and-deployment/images/boldbi-startup.png)
* Follow the steps in the link to do the [application startup](https://help.boldbi.com/application-startup/).



