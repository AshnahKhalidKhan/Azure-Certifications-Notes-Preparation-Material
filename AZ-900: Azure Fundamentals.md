# AZ-900: Azure Fundamentals

### Cloud Deployment Models
- **Public**:
  - Applications can be provisioned and deprovisioned quickly.
  - Organizations only pay for what they use.
- **Private**:
  - Hardware must be purchased.
  - The company has control over physical resources and security.
  - Customer is responsible for storage, VMs and runtime.
- **Hybrid**:
  - A hybrid cloud environment can be used to allow a private cloud to surge for increased, temporary demand by deploying public cloud resources.
  - Can be used to provide an extra layer of security i.e. users can flexibly choose which services to keep in public cloud and which to deploy to their private cloud infrastructure.
  - this cloud model uses some datacenters focused on providing cloud services to anyone that wants them, and some data centers that are focused on a single customer
- **Multi-cloud**:
  - two (or more) public cloud providers and manage resources and security in both environments.
- **Adantages of cloud computing over on-premises deployment:** scaling more quickly.
- **Compute + storage:** two services provided by all cloud providers.
- **Colocation:** business rents space in a shared physical datacenter.
- **Application Development:** responsibility of customer and typically done in-house or via a third party.

- **Capital Exepnditure (CapEx):** Upfront costs incurred one time e.g. hardware purchases.
- **Operational Exepnditure (OpEx):** Billed as you go; no upfront costs.
- **Geo-location:** allows you to deploy applications to regional datacenters across the world.
- **Geo-distribution:** ensuring customers have the best performance in their region by deploying apps and data to regional datacenters across the world.


###
- **Agility:** Deploying and configuring resources quickly as business requirements change.
- **Scalability:** Add RAM, CPU or entire VMs to a configuration.
- **Horizontal scaling:** Increasing compute capacity by adding instances of resources (e.g. additional virtual machine).
- **Vertical scaling:** Increasing RAM or CPU of an existing resource.
- **Elasticity:** configure auto-scaling so apps always have the resources they need to meet customer demand.
- **High Availability:** provide continuous user experience with no apparent/minimal downtime even when things go wrong; depends on SLA chosen.
- **Disaster Recovery:** Keeping data and other assets safe in the event of a disaster.
- **Reliability:** Ability of a system to recover from failures and continue functioning.
- **Cost Predictability:**
- **Performance Predictability:** Concepts supporting performance predictability include autoscaling, load balancing, and high availability.

### Shared Responsibility Model
 - **Applications**:
  - IaaS: you are fully responsible for deploying applications.
  - PaaS: Microsoft manages parts of the application stack, but you're responsible for application configuration, code security, and access controls.
  - SaaS: Microsoft manages parts of the application stack, but you're responsible for application configuration, code security, and access controls.
 - **Network Controls**:
  - IaaS: you configure all network security including firewalls and network segmentation.
  - PaaS: Microsoft provides baseline network security, but you configure application-level network controls.
  - SaaS: Microsoft manages network security.
 - **Client Devices**:
  - IaaS: you're fully responsible for endpoint protection and compliance.
  - PaaS: you're fully responsible for endpoint protection and compliance.
  - SaaS: Microsoft may provide some device management capabilities, but you're responsible for endpoint protection and compliance.
- **On-premises:**
  - Customer responsible for managing OS and applications.
- **IaaS:**
  - Examples: Azure VMs, VNETs, Azure Disk Storage.
  - Most control over hardware/managing physical servers.
  - Customer responsible for managing OS and applications, VMs and runtime.
  - Uses consumption-based, pay-as-you-go model.
  - Places the most responsibility on the customer
  - Ideal when you want total control over OS, the ability to run custom software and to use custom hosting configurations.
  - **Uses:**
    - Lift-and-shift migration: You’re setting up cloud resources similar to your on-prem datacenter, and then simply moving the things running on-prem to running on the IaaS infrastructure.
    - Testing and development: You have established configurations for development and test environments that you need to rapidly replicate. You can start up or shut down the different environments rapidly with an IaaS structure, while maintaining complete control.
- **PaaS:**
  - Examples: Azure SQL Database, Azure App Services, Azure Cosmos DB, Azure Monitor, Azure Functions, and Azure Storage..
  - Do not control OS and do not configure underlying servers.
  - Cloud provider is responsible for managing OS and physical network.
  - Customer is responsible for managing accounts, identities, information and data and user access.
  - Create a platform to host a software/create custom application yourself.
  - Used when needed to focus on application development.
  - OS is not accessible by customer.
  - Uses consumption-based, pay-as-you-go model.
  - **Uses:**
    - PaaS provides a framework that developers can build upon to develop or customize cloud-based applications.
    - PaaS lets developers create applications using built-in software components.
    - Tools provided as a service with PaaS allow organizations to analyze and mine their data, finding insights and patterns and predicting outcomes to improve forecasting, product design decisions, investment returns, and other business decisions.
- **SaaS:**
  - Example: MS Office 365, Dynamics 365.
  - With SaaS, you’re essentially renting or using a fully developed application.
  - Use software hosted on cloud.
  - Customer does not manage OS.
  - Cloud provider is responsible for managing OS and all aspects of the application environment.
  - OS is not accessible by customer.
  - Customer is responsible for data and access.
  - Typically, one version of the application is used by all customers.
  - Licensed through a monthly/annual subscription.
  - Software is centrally hosted and managed for all users/customers.
  - **Uses:**
    - Email and messaging.
    - Business productivity applications.
    - Finance and expense tracking.
- **ALWAYS RESPONSIBLE NO MATTER WHAT IAAS, SAAS, PAAS OR ON-PREMISES**:
  - **Data**: data classification, data protection, encryption decisions, and compliance with data governance requirements.
  - **Endpoints**: protecting client devices and endpoints that access your cloud services, including mobile devices, laptops, and desktops.
  - **Accounts**: creating, managing, and removing user access and accounts.
  - **Access Management**: implementing and managing access controls, including RBAC, MFA, and conditional access policies. 
- **AI Shared Responsibility**:
  - Microsoft is responsible for securing the AI infrastructure, model hosting, and platform-level safeguards.
  - Customers, however, remain accountable for how AI is applied within their environment—this includes protecting sensitive data, managing prompt security, mitigating prompt injection risks, and ensuring compliance with organizational and regulatory requirements.

###
- **Total Costs of Ownership (TCO) Calculator:**
  - Estimate the cost savings over time of operating a solution in Azure compared to an on-premises datacenter.
  - Example: compare costs of running an app in an on-premises datacenter with the costs of running the application in Azure.
- **Azure Pricing Calculator:** used to estimate costs for based on resource requirements.
- Factors affecting Azure costs: resource location and resource usage.
- Resource usage: CPU time, disk size, write operations.
- Deleting/deallocating resources stops billing for it.
- Costs are same no matter time of day or day of the the week.
- **Azure Reservations:** Up to **72% discount** on several resources with consistent usage for a long period of time without reducing functionality of the resource.
- **Spending limits:** Suspend a subscription when spending limit is reached.

###
- **Azure Arc:**
  - simplifies governance and management by delivering a consistent multi-cloud and on-premises management platform.
  - E.g. manage servers across third-party cloud platforms and on-premises environments.
  - Azure Arc can help manage your cloud environment whether it's a public cloud solely on Azure, a private cloud in your datacenter, a hybrid configuration, or even a multi-cloud environment running on multiple cloud providers at once.
 - **Azure VMware Solutions**:
  - VMware in a private cloud environment but want to migrate to a public or hybrid cloud? Azure VMware Solution lets you run your VMware workloads in Azure with seamless integration and scalability.
  - service developed by Microsoft in partnership with VMware, allowing organizations to migrate VMware-based workloads from on-premises to Azure.
  - allows for gradual migration to the cloud, with integration options for native Azure services such as Log Analytics, Microsoft Defender for Cloud, and Azure Backup Server.
  - Customers can modernize applications running on VMware over time through integration with Azure native management, security, and services.
  - also provides high availability and business continuity options because service has built-in redundancy with no single point of failure.
  - Utilization of existing VMware investments without the need for retraining.
  - Operational consistency for administrators and businesses, reducing change management.
  - A single point of support from Microsoft, simplifying licensing.
  - The ability to maximize existing Windows Server and SQL Server licenses through Azure Hybrid Benefit.
  - accelerate migration and minimize downtime by using the latest VMware Hybrid Cloud Extension (HCX) Enterprise functionality for large-scale, live migration from on-premises to Azure.
  - **Azure NetApp Files** is a native Azure service can be used to mount virtual machine (VM) file shares using server message block (SMB) or network file system (NFS).
- **Microsoft Purview:**
  - Data Catalog - enables data discovery.
  - Data Sharing - shares data within and between organizations.
  - Data Estate Insights - accesses data estate health.
  - Data Policy - governs access to data/used to manage access to data sources and datasets.
- **Management Groups:** manage access, policies and compliance across __**multiple subscriptions.**__ Management groups can be nested (one management group within another).
- 10,000 management groups can be supported in a single directory.
- A management group tree can support up to six levels of depth. This limit doesn't include the root level or the subscription level.
- Each management group and subscription can support only one parent.
- **Administrative Units:** delegate administration of Microsoft Entra resources such as users and groups.
- **Azure Policy:**
  - enforce company standards on Azure resources.
  - manage policies that control or audit resources to ensure configurations stay compliant with corporate standards.
  - E.g. enforce MFA on all accounts with write permissions.
  - E.g. ensure development team only creates VMs of a specific size.
  - E.g. restrict the deployments of VMs to a specific region.
- **Azure RBAC:**
  - Applied to a scope.
  - Scope is a resource or set of resources to which access is applied to.
- **Resource Locks:** prevent the accidental change or deletion of a resource.
- **Resource Tags:**
  - locate and act on resource associated with a specific workloads, environments, business units, or owners.
  - associate different resources without changing their locations.
  - associate costs with different environments.
  - categorizing costs by department.
- **Resource Groups:** logical container used to combine and organize Azure resources. When an action or setting at the Resource Group level is applied, the setting is applied to current and future resources.

###
- **Azure Cloud Shell:** Azure portal tool to manage Azure environment.
- **Azure CLI:**
  - executes commands in Bash that call Azure REST API.
  - preferable for Linux administrators.
- **Azure PowerShell:** executes commands in PowerShell.
- You can quickly change between PowerShell and BASH in the CLI by selecting the Switch to ... button or entering BASH or PWSH.

###
- **Azure Resource Manager (ARM) Templates:**
  - deployment and management service for Azure.
  - __**Parallel and idempotent**__ creation of Azure resources.
  - Defines application's infrastruction requirments.
  - Includes a validation step to ensure all resources are created in an order based on dependencies. 
  - Used for repeatable deployments done in a consistent matter.
  - Provides a management layer that accepts requests from any Azure tool or API.
- **Azure Functions:**
  - Execute code in a serverless environments.
  - Run code as a service without having to manage the underlying platform or infrastructure.
- **Azure Logic Apps:** similar to Azure Functions but uses predefined workflows instead of developing your own code.

###
- **Azure Service Health:**
  - Review root cause analysis (RCA) report for service outages.
  - Notification of service outages in a specific Azure region.
  - Information about planned maintenance for Azure services.
  - When a reboot is required for a service, it will allow you to choose when to perform the maintenance to minimize downtime.
- **Health Advisories:**
  - Issues that require you to take __**proactive**__ action to avoid service interruptions.
  - Should proactively review and act on to avoid __**service retirements**__ and __**breaking changes**__.
- **Service Issues:**
 - Issues that require __**immediate**__ action such as outages.

###
- Some services or virtual machine (VM) features are only available in certain regions, such as specific VM sizes or storage types.
- There are also some global Azure services that don't require you to select a particular region, such as Microsoft Entra ID, Azure Traffic Manager, and Azure DNS.
- A region is a geographical area on the planet that contains at least one, but potentially multiple datacenters.
- **Geography:**
- **Region Pairs:**
  - Replicate resources across a geography to ensure business continuity during a natural disaster at the primary site.
  - A region which is paired with another region in the same geography.
  - Each region is at least 300 miles away.
  - Most regions are paired in two directions, meaning they are the backup for the region that provides a backup for them e.g. West US and East US.
  - Some regions are paired in only one direction, meaning the Primary region does not provide backup for its secondary region e.g. West India's secondary region is South India, but South India's secondary region is Central India.
- **Sovereign Regions:**
  - Sovereign regions are instances of Azure that are isolated from the main instance of Azure.
  - US DoD Central, US Gov Virginia, US Gov Iowa and more: These regions are physical and logical network-isolated instances of Azure for U.S. government agencies and partners. These datacenters are operated by screened U.S. personnel and include additional compliance certifications.
  - China East, China North, and more: These regions are available through a unique partnership between Microsoft and 21Vianet, whereby Microsoft doesn't directly maintain the datacenters.
- **Availability Sets:** enhance resilience and high availability by staggering updates and varying power/network connectivity. They group VMs into update domains (for staggered updates) and fault domains (to protect against power/network failures). There is no additional cost for configuring availability sets; you only pay for the VM instances created. Update domain: The update domain groups VMs that can be rebooted at the same time. Fault domain: The fault domain groups your VMs by common power source and network switch. By default, an availability set splits your VMs across up to three fault domains.
- **Azure Virtual Machine Scale Sets:** deploy, manage and scale a set of identical VMs. Azure automates configuration, monitoring, and scaling of VMs based on demand or a defined schedule. They include a load balancer to optimize resource usage and are suitable for large-scale services like compute and big data.
- **Availability Zones:**
  - Physically separate datacenters within an Azure region, equipped with independent power, cooling and networking.
  - Primarily for VMs, managed disks, load balancers and SQL databases.
  - Availability zones are connected through high-speed, private fiber-optic networks.
  - To ensure resiliency, a minimum of three separate availability zones are present in all availability zone-enabled regions. However, not all Azure Regions currently support availability zones.
- Azure services that support availability zones fall into three categories:
  - Zonal services: You pin the resource to a specific zone (for example, VMs, managed disks, IP addresses).
  - Zone-redundant services: The platform replicates automatically across zones (for example, zone-redundant storage, SQL Database).
  - Non-regional services: Services are always available from Azure geographies and are resilient to zone-wide outages as well as region-wide outages.
- **Defence In Depth:**
  - use several layers of protection to prevent information from being accessed by unauthorized users.
  - uses a series of mechanisms to slow the advancement of an attack to gain unauthorized access to data.
- **Disaster Recovery Plan:** includes features like cloud-based backup, data replication and geo-distribution, to keep data safe in the event of a disaster.

###
- **Azure Virtual Desktop:**
  - cloud-based desktop and application virtualization service that allows users to access a cloud-hosted version of Windows from any location. This flexibility is essential for remote work scenarios, enabling users to maintain productivity regardless of their physical location.
  - It operates across various devices and operating systems, allowing access through remote desktops or modern browsers, which enhances usability and accessibility for users.
  - The service enhances security with centralized management through Microsoft Entra ID, which enables MFA and RBACs to secure user sign-ins. This centralized approach is vital for organizations aiming to protect sensitive information and manage user access effectively.
  - Azure Virtual Desktop separates data and applications from local hardware, significantly reducing the risk of confidential data being left on personal devices. This separation ensures that sensitive information is stored securely in the cloud rather than on potentially insecure local machines.
  - It supports multi-session deployment of Windows 10 or Windows 11 Enterprise, allowing multiple concurrent users on a single VM, which optimizes resource usage and cost efficiency for organizations.
  - This service provides a consistent user experience with broader application support compared to Windows Server-based operating systems, making it an attractive option for businesses that rely on diverse applications.
  - Additionally, Azure Virtual Desktop isolates user sessions in both single and multi-session environments, further enhancing security and usability, which is crucial for maintaining a secure and efficient virtual workspace.
  - lets you use Windows 10 or Windows 11 Enterprise multi-session, the only Windows client-based operating system that enables multiple concurrent users on a single VM.

###
- **Azure Advisor:**
  - Recommendations for reducing Azure costs.
  - Recommendations to help improve reliability, security, performance, achieve operational excellence and reduce costs.

###
- **Azure Monitor:**
  - Platform that collects metric and logging data.
  - Can be used to trigger auto-scaling using thresholds.
- **Application Insights:**
  - Automatically detect performance anomalies for web apps.
  - Use built-in analytics to see what users do on an app.

###
- **Azure Container Instances** & **Azure Kubernetes Service (AKS):**
  - Run applications in containers (virtualization environment).
  - Do not need to manage the OS for a container.

###
- **Azure Storage Accounts:**
  - **Azure Blob Storage:** store unstructured files e.g. images, text and binary data.
  - **Azure Disk Storage:**
  - **Azure Queue Storage:**
  - **Azure Table Storage:**
  - **Azure Files:** fully managed fileshares accessible using __**Server Message Block (SMB)**__ and __**Network File System (NFS)**__ protocol.

###
- **Microsoft Entra:** Provides two services i.e. **authentication** and **SSO**.
- **SSO:** sign in one time and use that credential to access multiple resources and applications from different providers.
- **MFA:** prompted for an additional form of identification during sign-in.
- **Conditional Access:**
  - Allow/deny access to resources based on identity signals.
  - Can enforce access to certain applications is only allowed if users are using an approved client application only.
  - Can enforce uers sign in from a specific location only.
  - Can enforce whether or not MFA is required.
- **Device Management:** registration of devices on Entra.
- **Microsoft Entra Connect:**
  - sync identities from on-premises ADDS domain to Microsoft Entra tenant.
  - use SSO, MFA and SSPR (self-service password reset).
  - **SSPR** prevents users from using known compromised passwords.

###
- **Service Endpoints:** used to expose Azure services to a VNET e.g. Azure SQL DB to Azure VNET.
- **ExpressRoute**: used to connect an on-premises network to Azure.
- **Peering**: connect VNETs together.
- **NSGs:** configure inbound and outbound rules for VNETs and VMs.
- **VPN Gateway:**
  - Type of virtual network gateway.
  - Deployed to a dedicated subnet of a VNET.
  - Used to connect an on-premises datacenter to Azure VNET through __**Site-to-Site(S2S)**__ VPN connection.
