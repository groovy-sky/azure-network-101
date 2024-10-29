# Introduction to Azure Networking

![](/img/net_logo.png)
 
## 1. Common Public Cloud Service Types

* **PaaS** (Platform as a Service): Provides a platform for developing, testing, and managing applications without the need to manage infrastructure.
* **SaaS** (Software as a Service): Delivers software applications over the internet on a subscription basis, eliminating the need for installation or management.
* **IaaS** (Infrastructure as a Service): Offers virtualized computing resources, including virtual machines, storage, and networks, giving users control over the operating system and applications.

## 2. Network Access Types for Azure Resources

Azure resources can have both private and public network access:

* **Private**: Resources are accessible only within a Virtual Network (VNet) or a specific subnet, ensuring secure communication within the private network.
* **Public**: Resources have an externally accessible IP address and can be reached from the public internet, suitable for web applications, APIs, or services requiring public accessibility.

## 3. Azure Network Fundamentals
 
Azure provides several network-related services and components to manage and secure network traffic:

| Icon | Name | Definition |
| --- | --- | --- |
| ![](/img/VNet.svg) | Virtual Network (**VNet**) | logically isolated network in Azure enabling secure communication between resources. |
| ![](/img/NSG.svg) | Network Security Group (**NSG**) | inbound and outbound access ruleset. |
| ![](/img/UDR.svg) | User-Defined Routing (**UDR**) | Customizing network traffic routing within Azure infrastructure, allowing specific routes for traffic flow, such as through virtual appliances or VPN gateways. |

## 4. IaaS Network Access
 
IaaS resources has private access by default(i.e. Virtual Network) and optionally can have public access. 

For example, to be able to run Azure VM you'll need configure a Network Interface Card (NIC) associated to Azure Virtual Network. By default, the NIC of a VM is connected to a specific subnet within the VNet, providing private access. This means that the VM can communicate with other resources within the same VNet but is not directly accessible from the public internet.

However, if you need to make the VM publicly accessible, you can associate a public IP address with the NIC. This allows the VM to have a publicly routable IP address, enabling external communication from the internet to the VM.

To control and secure the access to the VM, you can apply Network Security Groups (NSGs) at both the VNet level and the NIC level.

## 5. PaaS Network Access

PaaS resources, such as web apps or databases, by default are publicly available.