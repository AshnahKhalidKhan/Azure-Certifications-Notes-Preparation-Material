# AZ-900: Azure Fundamentals

### Cloud Deployment Models
- **Public**:
  - Applications can be provisioned and deprovisioned quickly.
  - Organizations only pay for what they use.
- **Private**:
  - Hardware must be purchased.
  - The company has control over physical resources and security.
- **Hybrid**:
- **Adantages of cloud computing over on-premises deployment:** scaling more quickly.
- **Compute + storage:** two services provided by all cloud providers.
- **Colocation:** business rents space in a shared physical datacenter.
- **Application Development:** responsibility of customer and typically done in-house or via a third party.
- **Capital Exepnditure (CapEx):** Upfront costs incurred one time e.g. hardware purchases.
- **Operational Exepnditure (OpEx):** Billed as you go; no upfront costs.

###
- **Agility:** Deploying and configuring resources quickly as business requirements change.
- **Scalability:** Add RAM, CPU or entire VMs to a configuration.
- **Horizontal scaling:** Increasing compute capacity by adding instances of resources (e.g. additional virtual machine).
- **Vertical scaling:** Increasing RAM or CPU of an existing resource.
- **Elasticity:** configure auto-scaling so apps always have the resources they need.
- **High Availability:** provide continuous user experience with no apparent/minimal downtime even when things go wrong.
- **Disaster Recovery:** Keeping data and other assets safe in the event of a disaster.

###
- **On-premises:**
  - Customer responsible for managing OS and applications.
- **IaaS:**
  - Examples: Azure VMs, VNETs.
  - Most control over hardware/managing physical servers.
  - Customer responsible for managing OS and applications.
  - Uses consumption-based, pay-as-you-go model.
- **PaaS:**
  - Examples: Azure SQL Database, Azure App Services, Azure Cosmos DB, Azure Monitor.
  - Do not control OS and do not configure underlying servers.
  - Cloud provider is responsible for managing OS.
  - Create a platform to host a software/create custom application yourself.
  - Used when needed to focus on application development.
  - OS is not accessible by customer.
  - Uses consumption-based, pay-as-you-go model.
- **SaaS:**
  - Example: MS Office 365.
  - Use software hosted on cloud.
  - Customer does not manage OS.
  - Cloud provider is responsible for managing OS.
  - OS is not accessible by customer.
  - Typically, one version of the application is used by all customers.
  - Licensed through a monthly/annual subscription.
  - Software is centrally hosted and managed for all users/customers.

###
- **Azure Pricing Calculator:** used to estimate costs for based on resource requirements.
- Factors affecting Azure costs: resource location and resource usage.
- Resource usage: CPU time, disk size, write operations.
- Deleting/deallocating resources stops billing for it.
- Costs are same no matter time of day or day of the the week.
- **Azure Reservations:** Up to **72% discount** on several resources with consistent usage for a long period of time without reducing functionality of the resource.
- **Spending limits:** Suspend a subscription when spending limit is reached.

###
- **Azure Policy:**
  - enforce company standards on Azure resources.
  - manage policies that control or audit resources to ensure configurations stay compliant with corporate standards.
  - E.g. enforce MFA on all accounts with write permissions.
  - E.g. ensure development team only creates VMs of a specific size.
- **Azure RBAC:**
  - Applied to a scope.
  - Scope is a resource or set of resources to which access is applied to.
- **Resource Locks:** prevent the accidental change or deletion of a resource.
- **Resource Tags:**
  - locate and act on resource associated with a specific workloads, environments, business units, or owners.
  - associate different resources without changing their locations.
- **Resource Groups:**

###
- **Azure Cloud Shell:** Azure portal tool to manage Azure environment.
- **Azure CLI:**
  - executes commands in Bash that call Azure REST API.
  - preferable for Linux administrators.
- **Azure PowerShell:** executes commands in PowerShell.

###
- **Azure Resource Manager (ARM) Templates:**
  - __**Parallel and idempotent**__ creation of Azure resources.
  - Defines application's infrastruction requirments.
  - Includes a validation step to ensure all resources are created in an order based on dependencies. 
  - Used for repeatable deployments done in a consistent matter.

###
- **Azure Service Health:**
  - Review root cause analysis (RCA) report for service outages.
  - Notification of service outages in a specific Azure region.
  - Information about planned maintenance for Azure services.
  - When a reboot is required for a service, it will allow you to choose when to perform the maintenance to minimize downtime.
- **Health Advisories:**
  - Issues that require you to take __**proactive**__ action to avoid service interruptions.
  - Should proactively review and act on to avoid service retirements and breaking changes.
- **Service Issues:**
 - Issues that require __**immediate**__ action such as outages.

###
- **Region Pairs:** replicate resources across a geography to ensure business continuity during a natural disaster at the primary site.
- **Availability Sets:**
- **Azure Virtual Machine Scale Sets:**
- **Availability Zones:**
- **Defence In Depth:** use several layers of protection to prevent information from being accessed by unauthorized users.
- **Disaster Recovery Plan:** includes features like cloud-based backup, data replication and geo-distribution, to keep data safe in the event of a disaster.

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
