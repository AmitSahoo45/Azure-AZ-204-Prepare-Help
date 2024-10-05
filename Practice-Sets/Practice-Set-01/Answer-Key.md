### Answer Key

1. a. No, the blob will be automatically moved back to cool storage the next day

explanation: Moving the blob from cool to hot does not modify it's modification date, and so it will be moved back to cool storage the next time lifecycle management runs. You need to either modify the rule to be based on last access date, or modify the file when moving it back so that the modification date is updated. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/storage/blobs/storage-lifecycle-management-concepts?tabs=azure-portal

---

2. a. function.json

The function.json file defines the function's trigger, bindings, and other configuration settings. Every function has one and only one trigger. The runtime uses this config file to determine the events to monitor and how to pass data into and return data from a function execution. The following is an example function.json file. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-triggers-bindings?tabs=csharp

---

3. b. Policies allow you to modify the behavior of the API using configuration instead of code. A policy can change both the inbound request and the outbound response.

explanation: Policies allow you to modify the inbound request as well as the outbound results without modifying the API code itself.

---

4. b. Core SQL

explanation: Core (SQL) API stores data in JSON document format. Cassandra API stores data in column-oriented schema. Gremlin API allows users to make graph queries and stores data as edges and vertices. MongoDB API also uses documents but is BSON format, which is a binary format and not text-based. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/cosmos-db/introduction

---

5. b. docker pull contoso.azurecr.io/marketing/website

explanation: By using repository namespaces, you can allow sharing a single registry across multiple groups within your organization. Registries can be shared across deployments and teams. Azure Container Registry supports nested namespaces, enabling group isolation. However, the registry manages all repositories independently, not as a hierarchy. The syntax is contoso.azurecr.io/marketing/website 

Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-registry/container-registry-best-practices#repository-namespaces

---

6. Create for them a Shared Access Signature (SAS)

explanation: Storage accounts are access by keys. Using SAS will let them have very granular access without exposing any other part of your storage account.

---

7. a. Change the applications to the same user-managed identity

explanation: Managed identities eliminate the need for developers to manage credentials. Managed identities provide an identity for applications to use when connecting to resources that support Azure Active Directory (Azure AD) authentication. Applications may use the managed identity to obtain Azure AD tokens. For example, an application may use a managed identity to access resources like Azure Key Vault where developers can store credentials in a secure manner or to access storage accounts. You cannot configure multiple applications to use the same system-assigned identity. You must use a user-assigned identity for this purpose. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/overview

---

8. c. az webapp log download

explanation: az webapp log download allows you to download the logs to your local disk. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/learn/modules/capture-application-logs-app-service/2-enable-and-configure-app-service-application-logging

---

9. b. Data that is repeatedly read

explanation: Data that is static but read frequently benefits most from being cached, because you can use the cache to retrieve the data instead of having to go back to the original data source every time. Data that is written and never read does not need to be cached since caching only benefits reading. Data that is always changing (like a stock price) cannot be cached since you always have to go back to the original source to retrieve the latest. Data that is infrequently read but is static can benefit from caching, but it does not benefit the most of the four options. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/architecture/best-practices/caching?toc=%2fazure%2fredis-cache%2ftoc.json

---

10. b. You don't have to check if the resource exists, you simply declare that it should exist

explanation: ARM templates allow you to create and deploy an entire Azure infrastructure declaratively. For example, you can deploy not only virtual machines but also the network infrastructure, storage systems, and any other resources you may need. 

Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/overview

---

11. c. logger.LogCritical("message");

explanation: logger.LogCritical("Message") writes a critical message at log level 5. Levels 4 and 5 are "error" messages. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/learn/modules/capture-application-logs-app-service/2-enable-and-configure-app-service-application-logging

---

12. a. Go into Azure Monitor. Go into Alerts. Select the Subscription scope. Select the Create or Update Container Registry signal. Add the action group that emails you. Give it a name and click save.

explanation: Azure Monitor can do this natively. You can create an Alert in Azure Monitor, based on the Create or Update Container Registry signal. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-registry/monitor-service

---

13. b. Performs a docker build and immediately pushes the result image into an ACR.

explanation: ACR Tasks is a suite of features within Azure Container Registry that provides streamlined and efficient Docker container image builds in Azure. az acr build is an ACR Task which queues a quick build, providing streaming logs for an Azure Container Registry. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-registry/container-registry-tutorial-quick-task

---

14. c. Service Bus

explanation: Service Bus Queue is enterprise-grade message queue.

---

15. a. Custom Handlers

explanation: Every Functions app is executed by a language-specific handler. While Azure Functions features many language handlers by default, there are cases where you may want to use other languages or runtimes. Custom handlers are lightweight web servers that receive events from the Functions host. Any language that supports HTTP primitives can implement a custom handler. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-custom-handlers

---

16. d. Azure File Sync

explanation: Azure File Sync service allows you to keep a local copy of files that are stored in the Azure File Shares in the cloud. While some users may opt to keep a full copy of their data locally, Azure File Sync additionally has the ability to transform Windows Server into a quick cache of your Azure file share. You can use any protocol that's available on Windows Server to access your data locally, including SMB, NFS, and FTPS. You can have as many caches as you need across the world. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/storage/file-sync/file-sync-introduction

---

17. a. Azure Container Registry (ACR)

explanation: You can send your container images to Azure Container Registry (ACR) to store them before deployment

--- 

18. d. File system, and blob storage

explanation: To route messages to log files, Azure Web apps use the Web server (IIS process). Because Windows-based Web apps are a well-established Azure service, and messaging for ASP.NET apps is tightly integrated with the underlying IIS service, Windows apps benefit from a rich logging infrastructure. For other apps, logging options may be limited by the development platform, even when running on a Windows app service. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/learn/modules/capture-application-logs-app-service/2-enable-and-configure-app-service-application-logging

19. b. Monitor pattern

explanation: The monitor pattern refers to a flexible, recurring process in a workflow. An example is polling until specific conditions are met. You can use a regular timer trigger to address a basic scenario, such as a periodic cleanup job, but its interval is static and managing instance lifetimes becomes complex. You can use Durable Functions to create flexible recurrence intervals, manage task lifetimes, and create multiple monitor processes from a single orchestration. An example of the monitor pattern is to reverse the earlier async HTTP API scenario. Instead of exposing an endpoint for an external client to monitor a long-running operation, the long-running monitor consumes an external endpoint, and then waits for a state change. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/durable/durable-functions-overview?tabs=csharp#monitoring

---

20. c. All of the data contained in Microsoft 365, including documents, calendar, email, Teams, and people.

explanation: Microsoft Graph is the gateway to data and intelligence in Microsoft 365. It provides a unified programmability model that you can use to access the tremendous amount of data in Microsoft 365, Windows 10, and Enterprise Mobility + Security. Microsoft Graph exposes REST APIs and client libraries to access data on the following Microsoft cloud services: (A) Microsoft 365 core services: Bookings, Calendar, Delve, Excel, Microsoft 365 compliance eDiscovery, Microsoft Search, OneDrive, OneNote, Outlook/Exchange, People (Outlook contacts), Planner, SharePoint, Teams, To Do, Workplace Analytics. (B) Enterprise Mobility and Security services: Advanced Threat Analytics, Advanced Threat Protection, Azure Active Directory, Identity Manager, and Intune. (C) Windows 10 services: activities, devices, notifications, Universal Print. (D) Dynamics 365 Business Central. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/graph/overview#whats-in-microsoft-graph


---

21. a. 3

explanation: Azure Storage always stores multiple copies of your data so that it is protected from planned and unplanned events, including transient hardware failures, network or power outages, and massive natural disasters. Redundancy ensures that your storage account meets its availability and durability targets even in the face of failures. Zone-redundant storage (ZRS) copies your data synchronously across three Azure availability zones in the primary region. For applications requiring high availability, Microsoft recommends using ZRS in the primary region, and also replicating to a secondary region. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/storage/common/storage-redundancy

---

22. d. Spot instances are significantly cheaper

explanation: Using Azure Spot Virtual Machines allows you to take advantage of our unused capacity at a significant cost savings. At any point in time when Azure needs the capacity back, the Azure infrastructure will evict Azure Spot Virtual Machines. Therefore, Azure Spot Virtual Machines are great for workloads that can handle interruptions like batch processing jobs, dev/test environments, large compute workloads, and more. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/virtual-machines/spot-vms

---

23. a. Any number or zero

explanation: You can mix and match different bindings to suit your needs. Bindings are optional and a function might have one or multiple input and/or output bindings. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-triggers-bindings?tabs=csharp

---

24. d. docker push myacr.azurecr.io/myimage

explanation: Use docker image push to share your images to the Docker Hub registry or a self-hosted one. You pass the URL of your ACR, which is in the format youruniquename.azurecr.io, plus the image name. 

Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-registry/container-registry-get-started-docker-cli?tabs=azure-cli#push-the-image-to-your-registry

---

25. b. System.Diagnostics.Trace.TraceError("message");

explanation: Logs messages generated by your application code. The messages can be generated by the web framework you choose, or from your application code directly using the standard logging pattern of your language. Each message is assigned one of the following categories: Critical, Error, Warning, Info, Debug, and Trace. You can select how verbose you want the logging to be by setting the severity level when you enable application logging. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/troubleshoot-diagnostic-logs

---

26. c. At 00:15, 00:30, and 00:45 (12:15am, 12:30am, and 12:45am); three times per day only.

explanation: CRON uses a "{second} {minute} {hour} {day} {month} {day-of-week}" format for expressions. The first "0" means that it runs when the second equals 0. The second "15,30,45" means when the minutes equal 15, 30 and 45. The third "0" means at midnight. So the answer is at 12:15, 12:30, and 12:45 every day. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-bindings-timer?tabs=csharp#ncrontab-expressions

---

27. c. `[resourceGroup().location]`

explanation: `[resourceGroup().location]` is the best answer because it accesses the resource group, and looks at the location parameter. The other answers do not do that. We don't know if the location is passed in as a parameter, and the requirement said the resource group location. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/template-functions-resource#resourcegroup

---

28. a. az acr import

explanation: As a recommended one-time step, import base images and other public content to your Azure container registry. The az acr import command in the Azure CLI supports image import from public registries such as Docker Hub and Microsoft Container Registry and from other private container registries. Refer to Microsoft Doc: https://docs.microsoft.com/en-ca/azure/container-registry/buffer-gate-public-content#import-images-to-an-azure-container-registry

29. c. 1 MB per second or 1000 events per second (whichever comes first)

explanation: 1 MB per second or 1000 events per second (whichever comes first)

---

30. b. Implement the Redis Cluster feature, and add a second shard to double the memory available.

explanation: Redis Cluster supports up to 10 shards to create 1.2 TB of memory.
