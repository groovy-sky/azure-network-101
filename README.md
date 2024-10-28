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

## 3. Azure Private Network Fundamentals
 
Azure provides several network-related services and components to manage and secure network traffic:

* **Virtual Network** (VNet): Logically isolated network in Azure enabling secure communication between resources.
* **Network Security Group** (NSG): inbound and outbound access ruleset.
* **User-Defined Routing** (UDR): Customizing network traffic routing within Azure infrastructure, allowing specific routes for traffic flow, such as through virtual appliances or VPN gateways.

## 4. IaaS Network Access
 
IaaS resources, like virtual machines, has private access by default(i.e. Virtual Network) and optionally can have public access.

## 5. PaaS Network Access

PaaS resources, such as web apps or databases, by default are publicly available.