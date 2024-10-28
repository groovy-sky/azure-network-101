# Introduction to Azure Networking

 
## 1. Common Public Cloud Service Types

* **PaaS (Platform as a Service): Provides a platform for developing, testing, and managing applications without the need to manage infrastructure.
* **SaaS (Software as a Service): Delivers software applications over the internet on a subscription basis, eliminating the need for installation or management.
* **IaaS (Infrastructure as a Service): Offers virtualized computing resources, including virtual machines, storage, and networks, giving users control over the operating system and applications.

## 2. Network Access Types for Azure Resources

 
Azure resources can have both private and public network access:

* **Private**: Resources are accessible only within a Virtual Network (VNet) or a specific subnet, ensuring secure communication within the private network.
* **Public**: Resources have an externally accessible IP address and can be reached from the public internet, suitable for web applications, APIs, or services requiring public accessibility.

## 3. Azure Network Fundamentals

 
Azure provides several network-related services and components to manage and secure network traffic:

* **Virtual Network** (VNet): Logically isolated network in Azure enabling secure communication between resources.
* **Network Security Group** (NSG): inbound and outbound access list.
* **User-Defined Routing** (UDR): Customizing network traffic routing within Azure infrastructure, allowing specific routes for traffic flow, such as through virtual appliances or VPN gateways.

## 4. IaaS Network Access

 
IaaS resources, like virtual machines, can have both private and public network access:

* **Private**: By default, IaaS resources are provisioned with a private IP address, communicating securely within the VNet or specific subnets.
* **Public**: IaaS resources can also have a public IP address, enabling accessibility from the public internet, suitable for web servers or remote access.

## 5. PaaS Network Access

PaaS resources, such as web apps or databases, typically have public network access:

* **Public Network Access: PaaS resources are designed to be accessed over the public internet, assigned with public endpoints for interaction from anywhere.
