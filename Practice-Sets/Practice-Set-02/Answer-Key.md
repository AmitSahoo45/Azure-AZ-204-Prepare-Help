### Answer Key

1. b. 6

Explanation: Azure Storage always stores multiple copies of your data so that it is protected from planned and unplanned events, including transient hardware failures, network or power outages, and massive natural disasters. Redundancy ensures that your storage account meets its availability and durability targets even in the face of failures. Geo-redundant storage (GRS) copies your data synchronously three times within a single physical location in the primary region using LRS. It then copies your data asynchronously to a single physical location in the secondary region. Within the secondary region, your data is copied synchronously three times using LRS. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/storage/common/storage-redundancy

---

2. b. logger.LogWarning("message");

Explanation: logger.LogWarning("Message") writes a warning message at log level 3. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/learn/modules/capture-application-logs-app-service/2-enable-and-configure-app-service-application-logging

---

3. d. A set of compute resources for a web app to run.

Explanation: In App Service (Web Apps, API Apps, or Mobile Apps), an app always runs in an App Service plan. In addition, Azure Functions also has the option of running in an App Service plan. An App Service plan defines a set of compute resources for a web app to run. These compute resources are analogous to the server farm in conventional web hosting. One or more apps can be configured to run on the same computing resources (or in the same App Service plan). Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/overview-hosting-plans

---

4. a. Custom Handlers

Explanation: Every Functions app is executed by a language-specific handler. While Azure Functions features many language handlers by default, there are cases where you may want to use other languages or runtimes. Custom handlers are lightweight web servers that receive events from the Functions host. Any language that supports HTTP primitives can implement a custom handler. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-custom-handlers

---

5. b. in, out, inout

Explanation: All triggers and bindings have a direction property in the function.json file. For triggers, the direction is always in. Input and output bindings use in and out. Some bindings support a special direction inout. If you use inout, only the Advanced editor is available via the Integrate tab in the portal. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-triggers-bindings?tabs=csharp

---

6. d. Azure Monitor

Explanation: Azure Monitor - a centralized dashboard that collects all the logs, metrics and events from your resources<br>See: <a href='https://docs.microsoft.com/en-us/azure/azure-monitor/overview'>https://docs.microsoft.com/en-us/azure/azure-monitor/overview</a>

---

7. b. Trace.TraceWarning("message");

Explanation: To log information to the app diagnostics log, use the System.Diagnostics.Trace class. There are four trace levels you can use, and these correlate with error, warning, information, and verbose logging levels shown in the Azure portal. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/learn/modules/capture-application-logs-app-service/2-enable-and-configure-app-service-application-logging

---

8. a. A list of publicly available Windows Server OS images in the EastUS region.

Explanation: A list of publicly available Windows Server OS images in the EastUS region. There could be dozens of Windows VM images available to you. I get 62 when I run this command myself. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/virtual-machines/windows/tutorial-manage-vm

---

9. d. Log Analytics Workspace

Explanation: Log Analytics Workspace is required to collect logs and metrics<br>See: <a href='https://docs.microsoft.com/en-us/azure/azure-monitor/platform/manage-access'>https://docs.microsoft.com/en-us/azure/azure-monitor/platform/manage-access</a>


---

10. d. Set an expiration value on your keys

Explanation: Setting an expiration value for keys allows the system to keep the cache size smaller for you, and you never need to worry about reaching the maximum cache size. 

Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-cache-for-redis/cache-best-practices

---

11. b. Core Tools, cross-platform on Windows, macOS and Linux

Explanation: Azure Functions Core Tools provides the core runtime and templates for creating functions, which enable local development. Version 2.X supports development on Windows, Linux and MacOS. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-develop-local

---

12. Switch the queue to "at-most-once" delivery

Explanation: At-most-once delivery is designed for this

---

13. c. At-most-once delivery is designed for this

Explanation: Azure Key Vault is a service that provides centralized secrets management, with full control over access policies and audit history. In order to read secrets from Key Vault, you need to have a vault created and give your app permission to access it. You must create a managed identity and assign it permissions to read the vault, or you can use a user-assigned identity. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/overview-managed-identity?tabs=dotnet

---

14. b. Every 5 minutes

Explanation: CRON uses a "{second} {minute} {hour} {day} {month} {day-of-week}" format for expressions. The first "0" means that it runs when the second equals 0. The second "*/5" means every 5th minute of every hour, of every day. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-bindings-timer?tabs=csharp#ncrontab-expressions

---

15. d. ASP.NET Core

Explanation: ASP.NET Core is a cross-platform version of ASP.NET. Ruby and Python are only natively supported on Linux. ASP.NET 4 is only supported on Windows. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/overview

---

16. d. At midnight on Jan 1st only

Explanation: CRON uses a "{second} {minute} {hour} {day} {month} {day-of-week}" format for expressions. The first "0" means that it runs when the second equals 0. The first three "0" means 0:00 or midnight. The fourth "1" means on the 1st day of the month. The fifth "1" means January. So the function triggers once per year, on Jan 1 at midnight. Happy new year! Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-bindings-timer?tabs=csharp#ncrontab-expressions

---

17. c. You can save a lot of money if you don't use the resource often as opposed to having it available for use 24/7

Explanation: Consumption-Based Model - paying for something based on how much you used, as opposed to paying for something no matter if you use it or not. <br>See: <a href='https://docs.microsoft.com/en-us/azure/azure-functions/functions-consumption-costs'>https://docs.microsoft.com/en-us/azure/azure-functions/functions-consumption-costs</a>

---

18. a. Unlimited

Explanation: Cosmos DB can store an unlimited amount of data. There is no specific limit.

---

19. c. Docker images, OCI images, OCI artifacts, Helm charts

Explanation: The following Docker container image formats are supported: Docker images, OCI images, OCI artifacts, Helm charts Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-registry/container-registry-image-formats

---

20. c. File system only

Explanation: To route messages to log files, Azure Web apps use the Web server (IIS process). Because Windows-based Web apps are a well-established Azure service, and messaging for ASP.NET apps is tightly integrated with the underlying IIS service, Windows apps benefit from a rich logging infrastructure. For other apps, logging options may be limited by the development platform, even when running on a Windows app service. The logging functionality available to Linux-based scripted apps, such as Node, is determined by the Docker image used for the app's container. Basic logging, using redirections to STDERR or STDOUT, uses the Docker logs. Richer logging functionality is dependent on the underlying image, such as whether this is running PHP, Perl, Ruby, and so on. To download equivalent Web application logging as provided by IIS for Windows apps, may require connecting to your container using SSH. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/learn/modules/capture-application-logs-app-service/2-enable-and-configure-app-service-application-logging


---

21. b. Stores data in memory

Explanation: Redis Cache uses memory (RAM) to store your information which allows it almost instant retrieval. As a result, there is an upper limit to the amount of data a single Redis node can store, and then you must cluster nodes to go above it. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/architecture/best-practices/caching?toc=%2fazure%2fredis-cache%2ftoc.json

---

22. d. You don't need to worry about the order of operations to create resources (dependencies), Azure takes care of creating them in the correct order

Explanation: You don't have to worry about the complexities of ordering operations. Resource Manager orchestrates the deployment of interdependent resources so they're created in the correct order. When possible, Resource Manager deploys resources in parallel so your deployments finish faster than serial deployments. You deploy the template through one command, rather than through multiple imperative commands. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/overview

---

23. b. mycontainer.(azureregion).azurecontainer.io

Explanation: Azure Container Instances enables exposing your container groups directly to the internet with an IP address and a fully qualified domain name (FQDN). When you create a container instance, you can specify a custom DNS name label so your application is reachable at customlabel.azureregion.azurecontainer.io. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-instances/container-instances-overview

---

24. a. Retry attempts will delay based on a backoff strategy, where each attempt will increase the duration that it waits before retrying.

Explanation: Exponential = Retry attempts will delay based on a backoff strategy, where each attempt will increase the duration that it waits before retrying. Fixed = Retry attempts happen at fixed intervals; each delay is a consistent duration. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/dotnet/api/azure.core.retrymode?view=azure-dotnet

---

25. a. Resource Group

Explanation: Each resource can exist in only one resource group. However, you can move a resource from one resource group to another group. The resources inside the resource group do not have to exist in the same region as the resource group. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/overview

---

26. b. Eviction

Explanation: VMs can be evicted based on capacity or the max price you set. When creating an Azure Spot Virtual Machine, you can set the eviction policy to Deallocate (default) or Delete. As well, pricing is variable. Even though there is no SLA (for obvious reasons), this is not the major risk to using spot instances. Your account is limited to the number of any instance type you have per region, and so the limit on spot instances is not different than that. They should cost less than regular VMs though. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/virtual-machines/spot-vms

---

27. d. Gremlin API

Explanation: Gremlin API allows users to make graph queries and store data as edges and vertices. Cassandra API stores data in a column-oriented schema. Core (SQL) API stores data in document format. Table API stores data in key/value format. 

Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/cosmos-db/introduction

--- 

28. a. az acr build

Explanation: ACR Tasks is a suite of features within Azure Container Registry that provides streamlined and efficient Docker container image builds in Azure. az acr build is an ACR Task which queues a quick build, providing streaming logs for an Azure Container Registry. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-registry/container-registry-tutorial-quick-task

---

29. b. az acr build

Explanation: az acr build is a ACR Task. ACR Tasks is a suite of features within Azure Container Registry that provides streamlined and efficient Docker container image builds in Azure. Because ACR tasks use docker build to build your images, no changes to your Dockerfiles are required to start using ACR Tasks immediately. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-registry/container-registry-tutorial-quick-task

---

30. a. The first available private IP address in the Subnet1 address range

Explanation: A virtual machine (VM) is automatically assigned a private IP address from a range that you specify, based on the subnet in which the VM is deployed. The VM retains the address until the VM is deleted. Azure dynamically assigns the next available private IP address from the subnet you create a VM in. If you want a specific IP address from the subnet assigned to the VM, assign a static IP address. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/virtual-network/virtual-networks-static-private-ip-arm-pportal
