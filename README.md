# Azure-Web-App-Terraform-Setup
Provisioning Azure Web App Basic Infrastructure with Terraform
## Project Overview

This project provisions the following Azure resources:

- **Resource Group**: A container that holds related resources.
- **Virtual Network (VNet)**: A virtual network for the infrastructure.
- **Subnet**: A logical subdivision of the virtual network.
- **Public IP Address**: Allows inbound connections to the virtual machine.
- **Network Interface (NIC)**: Connects the VM to the VNet.
- **Network Security Group (NSG)**: Secures the network interface by allowing inbound HTTP and HTTPS traffic.
- **Linux Virtual Machine (VM)**: A virtual machine running Ubuntu, with Nginx installed and configured to start on boot.

## Terraform Code

The Terraform code in this repository sets up the infrastructure as follows:

1. **Resource Group**: Defined using `azurerm_resource_group`.
2. **Virtual Network and Subnet**: Created using `azurerm_virtual_network` and `azurerm_subnet`.
3. **Public IP Address**: Provisioned with `azurerm_public_ip`.
4. **Network Interface**: Configured with `azurerm_network_interface`.
5. **Network Security Group**: Secures the VM by allowing HTTP (port 80) and HTTPS (port 443) traffic.
6. **Linux Virtual Machine**: A VM is created with Nginx installed via custom data.
