### Answer Key

1. c. Data that remains relatively static

Explanation: Data that is static benefits most from being cached, because you can use the cache to retrieve the data instead of having to go back to the original data source every time. Data that is written and never read does not need to be cached since caching only benefits reading. Data that is only ever used once by a session does not need to be cached as well since the first time the data is read, you have to go to the original source. So if you never need it a second time, you don't need to cache it. And data that is always changing (like a stock price) cannot be cached since you always have to go back to the original source to retrieve the latest. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/architecture/best-practices/caching?toc=%2fazure%2fredis-cache%2ftoc.json

---

2. a. 12 hours

Explanation: App logs are the output of runtime trace statements in app code. For example, you might want to check some logic in your code by adding a trace to show when a particular function is being processed, or you might only want to see a logged message when a particular level of error has occurred. App logging is primarily for apps in pre-production and for troublesome issues, because excessive logs can carry a performance hit and quickly consume storage; for this reason, logging to the file system is automatically disabled after 12 hours. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/learn/modules/capture-application-logs-app-service/2-enable-and-configure-app-service-application-logging

---

3. b. LRS

Explanation: Azure Storage always stores multiple copies of your data so that it is protected from planned and unplanned events, including transient hardware failures, network or power outages, and massive natural disasters. Redundancy ensures that your storage account meets its availability and durability targets even in the face of failures. Locally redundant storage (LRS) copies your data synchronously three times within a single physical location in the primary region. LRS is the least expensive replication option, but is not recommended for applications requiring high availability or durability. Refer to Microsoft Doc: https://azure.microsoft.com/en-ca/pricing/details/storage/blobs/

---

4. d. container create

Explanation: az container create will create a new container instance. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-instances/container-instances-quickstart

---

5. b. Microsoft.Resources/deployments

Explanation: To deploy complex solutions, you can break your Azure Resource Manager template (ARM template) into many related templates, and then deploy them together through a main template. The related templates can be separate files or template syntax that is embedded within the main template. To link a template, add a deployments resource to your main template. In the templateLink property, specify the URI of the template to include. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/linked-templates?tabs=azure-powershell

---

6. b. Inbound

Explanation: Authentication is an inbound policy. Requests that fail to authenticate do not have the requests passed on to the API backend at all. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/api-management/api-management-authentication-policies

---

7. a. https://(app-name).scm.azurewebsites.net

Explanation: Kudu is the engine behind a number of features in Azure App Service related to source control based deployment, and other deployment methods like Dropbox and OneDrive sync. App not in Isolated tier uses https://(app-name).scm.azurewebsites.net, while apps in the isolated tier use https://(app-name).scm.(ase-name).p.azurewebsites.net. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/resources-kudu

---

8. a. Ensure that the client is always routed to the same instance for the life of the session.

Explanation: ARR affinity: In a multi-instance deployment, ensure that the client is routed to the same instance for the life of the session. You can set this option to Off for stateless applications. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/configure-common

---

9. b. ASPNETCORE_ENVIRONMENT="Development"

Explanation: The development environment can enable features that shouldn't be exposed in production. If the environment isn't set, it defaults to Production, which disables most debugging features. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/configure-language-dotnetcore?pivots=platform-windows#access-environment-variables

---

10. b. F-series VMs provide higher performance (ACU) per virtual CPU compared to D-series

Explanation: The best advantage of the F-series VMs is that they provide faster performance per virtual CPU than the D-series. The machine hardware is designed for CPU performance. Pricing is actually comparable. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/virtual-machines/acu

---

11. a. It moves your App Service plan to a higher pricing tier, giving you more CPU, memory, disk space and extra features.

Explanation: Scale up: Get more CPU, memory, disk space, and extra features like dedicated virtual machines (VMs), custom domains and certificates, staging slots, autoscaling, and more. You scale up by changing the pricing tier of the App Service plan that your app belongs to. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/manage-scale-up

---

12. a. Cache-aside pattern

Explanation: The name gives it away. The Cache-Aside pattern is designed to load data on demand into a cache from a data store. This can improve performance and also helps to maintain consistency between data held in the cache and data in the underlying data store.  Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/architecture/patterns/cache-aside

---

13. c. Increases the number of VM instances that run your app.

Explanation: Scale out: Increase the number of VM instances that run your app. You can scale out to as many as 30 instances, depending on your pricing tier. App Service Environments in Isolated tier further increases your scale-out count to 100 instances. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/manage-scale-up

---

14. a. if (myTimer.IsPastDue)

Explanation: if (myTimer.IsPastDue) is the correct answer. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-bindings-timer?tabs=csharp#ncrontab-expressions

---

15. a. Trace.WriteLine("message");

Explanation: To log information to the app diagnostics log, use the System.Diagnostics.Trace class. There are four trace levels you can use, and these correlate with error, warning, information, and verbose logging levels shown in the Azure portal. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/learn/modules/capture-application-logs-app-service/2-enable-and-configure-app-service-application-logging

---

16. c. Create the shared access signature using a stored access policy

Explanation: A shared access signature (SAS) provides secure delegated access to resources in your storage account. With a SAS, you have granular control over how a client can access your data. A stored access policy is defined on a resource container, which can be a blob container, table, queue, or file share. The stored access policy can be used to manage constraints for one or more service shared access signatures. When you associate a service SAS with a stored access policy, the SAS inherits the constraints-the start time, expiry time, and permissions-defined for the stored access policy. You can modify the stored access policy at any time after the SAS has been created. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/storage/common/storage-sas-overview

17. b. No, each account can only contain one type of data

Explanation: The API determines the type of account to create. Azure Cosmos DB provides five APIs: Core (SQL) and MongoDB for document data, Gremlin for graph data, Azure Table, and Cassandra. Currently, you must create a separate account for each API. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/cosmos-db/account-databases-containers-items

---

18. d. az webapp log tail

Explanation: az webapp log will retrive the log, and the tail operator will read the last lines of the log and keep a live stream of it going. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/learn/modules/capture-application-logs-app-service/2-enable-and-configure-app-service-application-logging

---

19. b. Durable functions

Explanation: Durable Functions is an extension of Azure Functions that lets you write stateful functions in a serverless compute environment. The extension lets you define stateful workflows by writing orchestrator functions and stateful entities by writing entity functions using the Azure Functions programming model. Behind the scenes, the extension manages state, checkpoints, and restarts for you, allowing you to focus on your business logic. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/durable/durable-functions-overview?tabs=csharp

---

20. b. AppServiceHTTPLogs

Explanation: AppServiceHTTPLogs are web logs. AppServiceAppLogs are application logs. AppServiceAuditLogs contain login activity via FTP and kudu. And AllMetrics are not logs, but performance metrics. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/troubleshoot-diagnostic-logs

---

21. a. Exactly one

Explanation: Triggers are what cause a function to run. A trigger defines how a function is invoked and a function must have exactly one trigger. Triggers have associated data, which is often provided as the payload of the function. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-triggers-bindings?tabs=csharp

---

22. b. Set the ConsistencyLevel property of QueryRequestOptions when making the query.

Explanation: QueryRequestOptions.ConsistencyLevel Property gets or sets the consistency level required for the request in the Azure Cosmos DB service. This is a request level property, and doesn't affect the database settings. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/dotnet/api/microsoft.azure.cosmos.queryrequestoptions.consistencylevel?view=azure-dotnet#Microsoft_Azure_Cosmos_QueryRequestOptions_ConsistencyLevel

---

23. b. Three

Explanation: When you create an app in App Service, it is put into an App Service plan. When the app runs, it runs on all the VM instances configured in the App Service plan. If multiple apps are in the same App Service plan, they all share the same VM instances. If you have multiple deployment slots for an app, all deployment slots also run on the same VM instances. In this way, the App Service plan is the scale unit of the App Service apps. If the plan is configured to run five VM instances, then all apps in the plan run on all five instances. If the plan is configured for autoscaling, then all apps in the plan are scaled out together based on the autoscale settings. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/overview-hosting-plans

---

24. b. Control plane, Nodes

Explanation: A Kubernetes cluster is divided into two components: 1. Control plane: provides the core Kubernetes services and orchestration of application workloads. 2. Nodes: run your application workloads. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/aks/concepts-clusters-workloads

---

25. c. myprivateacr.azurecr.io

Explanation: azurecr.io is the general domain name for ACR, and myprivateacr.azurecr.io points to your own private registry (where myprivateacr is the name of your unique registry). Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-registry/container-registry-get-started-portal

---

26. c. Once every hour of the day, at 5 minutes after the hour

Explanation: CRON uses a "{second} {minute} {hour} {day} {month} {day-of-week}" format for expressions. The first "0" means that it runs when the second equals 0. The second "5" means it will run at 5 minutes past the hour. The third "*" means that it will run every hour of every day. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-bindings-timer?tabs=csharp#ncrontab-expressions

---

27. b. Configuration > General Settings

Explanation: You can set the specific version of Python in Configuration > General Settings. 

Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/configure-common

---

28. c. Strong consistency is that, across the world, readers are guaranteed to always get the most recent committed version of an item.

Explanation: Strong consistency is that, across the world, readers are guaranteed to always get the most recent committed version of an item. A client will never see a partially committed item. See docs: https://docs.microsoft.com/en-us/azure/cosmos-db/consistency-levels

---

29. c. ARM Templates

Explanation: As infrastructure has become part of the iterative process, the division between operations and development has disappeared. Teams need to manage infrastructure and application code through a unified process. To implement infrastructure as code for your Azure solutions, use Azure Resource Manager templates (ARM templates). The template is a JavaScript Object Notation (JSON) file that defines the infrastructure and configuration for your project. The template uses declarative syntax, which lets you state what you intend to deploy without having to write the sequence of programming commands to create it. In the template, you specify the resources to deploy and the properties for those resources. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/overview

30. b. Enable Always On setting on the General Settings page.

Explanation: Always On: Keeps the app loaded even when there's no traffic. When Always On is not turned on (default), the app is unloaded after 20 minutes without any incoming requests. The unloaded app can cause high latency for new requests because of its warm-up time. When Always On is turned on, the front-end load balancer sends a GET request to the application root every five minutes. The continuous ping prevents the app from being unloaded. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/configure-common
