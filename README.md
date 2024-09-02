# Azure Integration Project: Virtual Machine and Container Instances

## Team Members
1. Durga Warrier [1041940]
2. Kailash Bangari [1041751]
3. Mayank Mali [1041939]
4. Neeraj Chawla [1041416]

## Project Summary
This project illustrates the process of connecting an Azure Virtual Machine (VM) with Azure Container Instances (ACI) within a single Virtual Network (VNet). The objective is to establish secure communication between the VM and the containerized applications running in the ACI, all within the same VNet.

## Key Elements
- **Resource Group**: Organizes and manages Azure resources in a logical container.
- **Virtual Network (VNet)**: An isolated network environment in Azure where the VM and ACI coexist.
- **Virtual Machine (VM)**: A flexible, on-demand computing resource provided by Azure.
- **Azure Container Instances (ACI)**: A service enabling the deployment of containerized applications without managing infrastructure.
- **Networking Configuration**: Ensures secure communication between the VM and the ACI within the same network environment.

## Requirements
- An active Azure account
- Familiarity with the Azure Portal and basic networking concepts
- SSH or RDP client available on your local machine

## Deployment Steps

### 1. Setting Up a Resource Group
1. Access the Azure Portal.
2. Go to **Resource groups** from the menu.
3. Click **+ Create**.
4. Provide a name for the Resource Group.
5. Choose the appropriate **Subscription** and **Region**.
6. Click **Review + Create**, then proceed with **Create**.

### 2. Configuring a Virtual Network (VNet)
1. In the Azure Portal, navigate to **Virtual networks**.
2. Select **+ Create** to establish a new VNet.
3. Name the VNet and select the same **Subscription** and **Region** as your Resource Group.
4. Set up the **IP Address space** and **Subnets** according to your needs.
5. Click **Review + Create**, followed by **Create**.

### 3. Creating a Virtual Machine (VM)
1. Go to **Virtual machines** within the Azure Portal.
2. Select **+ Create** to set up a new VM.
3. Choose the **Resource Group** you created earlier.
4. Enter a name for the VM and specify the **Region**.
5. Select an **Operating System Image** (e.g., Windows or Linux).
6. Configure the **VM Size** and **Administrator credentials**.
7. Under **Networking**, ensure the VM is associated with the VNet you previously configured.
8. Click **Review + Create**, then click **Create**.

### 4. Launching Azure Container Instances (ACI)
1. Navigate to **Container instances** in the Azure Portal.
2. Click **+ Create** to launch a new container instance.
3. Select the same **Resource Group** and **Region** as your VM.
4. Provide a name for the container instance and select a container image from Docker Hub or Azure Container Registry.
5. Under **Networking**, ensure the container instance is connected to the same VNet and Subnet as your VM.
6. Click **Review + Create**, then click **Create**.

## Conclusion
By following these steps, you successfully integrated an Azure Virtual Machine with Azure Container Instances within a Virtual Network. This setup provides a secure and scalable environment for running both traditional VM workloads and modern containerized applications. The project demonstrates the flexibility and power of Azure's networking capabilities, enabling seamless communication and resource management within a cloud environment.
