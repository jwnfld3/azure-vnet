# Set Up a Virtual Network in Azure (Free Tier)

## Overview
In this lab, a **Virtual Network (VNet)** is created in Azure, which is a fundamental building block for cloud infrastructure. The VNet enables secure communication between Azure resources. The free-tier networking service allows 50GB of free egress data per month, making this lab cost-effective while learning about Azure networking.

---

## Lab Requirements
- **Azure Subscription**: A valid Microsoft Azure account (free or paid).
- **Internet Access**: For accessing the Azure portal.
- **Azure Portal Access**: An active login to the Azure portal.
- **Basic Understanding of Networking**: Familiarity with networking concepts such as IP addressing, subnets, and routing will help.

---

## Who
- **Target Audience**: IT professionals, cloud engineers, network administrators, and students interested in cloud networking.
- **Prerequisites**: Basic knowledge of networking and cloud platforms.

---

## What
- Create a **Virtual Network (VNet)** in Azure.
- Configure the VNet with at least one subnet.
- Learn how to connect other Azure resources to the VNet in later labs (e.g., Virtual Machines, Azure App Services).

---

## When
- **Estimated Time**: 30 minutes.
- **Best for**: Beginner to intermediate users wanting to understand networking in Azure.

---

## Where
- **Lab Location**: Azure portal (https://portal.azure.com).
- **Lab Environment**: Microsoft Azure cloud.

---

## Why
- A Virtual Network in Azure allows secure connections between Azure resources, enabling communication within a cloud environment.
- Understanding how to configure VNets is crucial for setting up infrastructure in the cloud and establishing secure networking.
- This knowledge is essential for managing scalable and secure cloud applications.

---

## Steps

### 1. Sign in to Azure Portal
- **Definition**: The Azure portal is a web-based interface that allows users to manage Azure resources. Access is granted through an Azure subscription.

### 2. Create a Virtual Network
1. In the left-hand menu, click on **Create a Resource**.
2. In the "New" window, type **"Virtual Network"** in the search bar and select **Virtual Network**.
3. Click **Create**.

   **Definition**: A Virtual Network (VNet) is a logical representation of a network in Azure that provides isolation, segmentation, and security for cloud resources.

### 3. Configure Virtual Network
- **Subscription**: Choose the active subscription.
- **Resource Group**: Select an existing resource group or create a new one.
- **Name**: Enter a name for the VNet (e.g., **MyFirstVNet**).
- **Region**: Select the Azure region closest to the intended users or target infrastructure.
- **Address Space**: Define the IP address range for the VNet (e.g., `10.0.0.0/16`).

   **Definition**: A resource group is a logical container used to group related Azure resources for easy management and billing. The address space defines the range of private IP addresses that the VNet will use.

### 4. Add Subnet
- **Subnet Name**: Enter a name for the subnet (e.g., **MyFirstSubnet**).
- **Subnet Address Range**: Define the IP range for the subnet (e.g., `10.0.0.0/24`).
  - Additional subnets can be added later if required.

   **Definition**: A subnet is a range of IP addresses in the VNet that are used to segment the network. This allows for network traffic isolation and management.

### 5. Review and Create
- Review all configurations to ensure the VNet is set up correctly.
- Click **Create** to deploy the Virtual Network.

   **Definition**: The **Review + Create** step allows validation of the configuration settings before final deployment of the VNet.

### 6. Verify the Virtual Network
- After the deployment process, navigate to **Virtual Networks** in the Azure portal to view the newly created VNet.
- Click on the VNet to check the details, including the address space and subnet configuration.

   **Definition**: Once deployed, a Virtual Network can be managed and monitored through the Azure portal, ensuring it is correctly configured and functioning.

### 7. Connect Resources (Optional)
- Virtual Machines and other Azure resources can now be connected to the VNet.
- To test connectivity, a Virtual Machine or Azure App Service can be created and associated with the VNet during setup.

   **Definition**: A Virtual Network is the foundation for connecting and isolating resources in Azure. Linking resources to the VNet ensures secure communication between them.

---

## Post-Lab
- **Resource Cleanup**: After completing the lab, delete the Virtual Network if it is no longer needed to avoid unnecessary charges. Navigate to **Resource Groups** and delete the entire resource group if it is not required.
- **Next Steps**: In subsequent labs, VNets will be used to connect resources, implement network security groups (NSGs), and manage network traffic.

---

## Conclusion
A **Virtual Network (VNet)** has been successfully created in Azure. This fundamental skill enables secure communication between Azure resources. Future labs will build on this knowledge to explore more advanced networking features like subnets, VPNs, and network security configurations.
