# Project: Managed Service for Microsoft Active Directory on Google Cloud

![Imgur](https://i.imgur.com/ypZ1yVh.jpg) 

## Learning Points

### 1. Provisioning Active Directory (AD) Servers using Google Cloud Marketplace

To start the project, you will need to provision Active Directory servers using the Google Cloud Marketplace. Here are the steps:

- Log in to your Google Cloud Console.
- Navigate to the **Marketplace** section.
- Search for the **Microsoft Active Directory** or a related solution.
- Choose an appropriate AD server instance and configuration.
- Follow the prompts to deploy the instance.

### 2. Deploy a Windows Virtual Machine

After provisioning the AD servers, you'll need to deploy a Windows virtual machine that will be added to the domain. Here's what you need to do:

- Access the Google Cloud Console.
- Go to the **Compute Engine** section.
- Create a new virtual machine instance.
- Choose Windows as the operating system.
- Configure the instance with appropriate resources and settings.
- Allow necessary firewall rules for communication.

### 3. Update DNS Settings for a Windows VM Instance

To ensure that your Windows virtual machine can communicate with the Active Directory servers, you need to update its DNS settings:

- Connect to the Windows VM using Remote Desktop Protocol (RDP).
- Open the **Network and Sharing Center**.
- Click on **Change adapter settings**.
- Right-click on the network adapter and select **Properties**.
- Select **Internet Protocol Version 4 (TCP/IPv4)** and click on **Properties**.
- Set the preferred DNS server to the IP address of your Active Directory server.
- Confirm and save the settings.

### 4. Add a Windows Virtual Machine to a Domain

Now that your VM is properly configured, you can add it to the Active Directory domain:

- From the Windows VM, open **System Properties**.
- Go to the **Computer Name** tab and click on **Change**.
- Select **Domain** and enter the name of your Active Directory domain.
- Provide credentials with sufficient privileges to join the domain.
- Restart the VM to apply the changes.
- After reboot, the VM will be part of the Active Directory domain.

## Conclusion

By following these learning points, you will have successfully set up a project involving Managed Service for Microsoft Active Directory on Google Cloud Platform. This project covers provisioning AD servers, deploying Windows VMs, configuring DNS settings, and adding VMs to the domain.
