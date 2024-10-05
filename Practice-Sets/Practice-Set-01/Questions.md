### Questions

1. You have a Lifecycle Storage policy that moves blobs from hot storage to cool storage if they have not been modified in 30 days. You realize that there is a frequently accessed file that is in cool storage due to this policy, and you'd like to save money by moving it back to hot storage. So you manually move this file back to hot storage. Will this solve your problem?
- a. No, the blob will be automatically moved back to cool storage the next day
- b. Yes

----

2. Azure Functions store their configuration settings in which file?
- a. function.json
- b. default.js
- c. web.config
- d. index.js

----

3. The API Management Gateway includes a powerful feature called Policies. What is the main function of policies?
- a. Increase the security of your account by rejecting traffic coming in to the API by IP address
- b. Policies allow you to modify the behavior of the API using configuration instead of code. A policy can change both the inbound request and the outbound response.
- c. You can set rules as to who has access to an API and who does not.
- d. Policies allow you to direct the incoming traffic to several back-end APIs to help balance the load of the request.

---

4. Which CosmosDB API format works best with document (JSON) data?
- a. Cassandra API
- b. Core SQL
- c. MongoDB API
- d. Graph API

---

5. You have an Azure Container Registry named 'contoso.azurecr.io'. There are several departments in your company that need to push images to the registry, and you want to keep them organized. You decide to use repository namespaces to separate out 'sales', 'marketing', 'technology' and 'customerservice'. How do you pull down the container image for the 'website' project located in the marketing namespace?
- a. docker pull marketing.contoso.azurecr.io/website
- b. docker pull contoso.azurecr.io/marketing/website
- c. docker pull contoso.azurecr.io -location marketing/website
- d. docker pull contoso.azurecr.io -path marketing -project website

---

6. What option do you have to grant someone access to a single container in your Azure storage account without having to give them your storage account keys?
- a. Recycle the storage account keys after giving one to them
- b. Grant their user contributor access to your storage account within your subscription
- c. Create for them a Shared Access Signature (SAS)
- d. Change the permission settings for the container to public

---

7. Your company has several applications running on Azure App Services - App1, App2, App3 and App4. Each application is configured to use a system-managed identity to access resources. Your applications all store their secrets in a KeyVault named KV1. You are finding it difficult to manage the permissions for all these applications, and would like to move to a single managed identity for all applications instead of each application having their own. What action do you take to implement that?
- a. Change the applications to the same user-managed identity
- b. Create one user in Azure Active Directory for all applications, and have the applications use that
- c. Change the applications to the same system-managed identity
- d. Create one user in Azure Active Directory for each application, and have the applications use that

---

8. What is the Azure CLI command to download application log files to the local disk?
- a. az webapp log
- b. az log download
- c. az webapp log download
- d. az webapp log tail

---

9. Which type of data can most benefit from being stored in a caching system like Azure Redis Cache?
- a. Data that is repeatedly written
- b. Data that is repeatedly read
- c. Data that is infrequently read but is static
- d. Data that is repeatedly read, and can return a different value every time

---

10. ARM templates are said to have a declarative syntax. Why is a declarative syntax better than a programmatic approach?
- a. Programmatic approach does not support advanced techniques such as loops, variables, parameters, and random resource names
- b. You don't have to check if the resource exists, you simply declare that it should exist
- c. Declarative syntax only requires minor changes to the code before each deployment to ensure uniqueness
- d. Declarative syntax compiles into a binary form and is quicker to deploy

---

11. In ASP.NET Core, using the logger factory class, how do you write a message to the application diagnostics log that only shows up with the user has enabled error level messages?
- a. logger.LogDebug("Message");
- b. logger.LogWarning("Message");
- c. logger.LogCritical("message");
- d. logger.LogTrace("Message");

---

12. You would like to receive an email every time a new Azure Container Registry is created. Which of the following steps would accomplish that goal?
- a. Go into Azure Monitor. Go into Alerts. Select the Subscription scope. Select the Create or Update Container Registry signal. Add the action group that emails you. Give it a name and click save.
- b. Create an Azure Automation Runbook that checks your Account every 15 minutes for new resources and alerts you as new ones are created.
- c. Using Azure Event Grid, you can connect into the Azure subscription to receive alerts for resources created. The Event Grid can filter those events to only Azure Container Registry, and call a Function.
- d. Azure Service Health can monitor your Azure account and Alert you when new resources are created on your account.

---

13. What does the CLI command 'az acr build --registry $ACR_NAME --image helloacrtasks:v1 .' do?
- a. Performs a docker build and keeps the image on the local machine
- b. Performs a docker build and immediately pushes the result image into an ACR.
- c. Creates a new ACR resource if one doesn't exist under that name, otherwise does nothing
- d. Creates a new ACR resource if one doesn't exist under that name, or deletes the images from the existing resource

---

14. You are a developer for Acme Inc. Your company's flagship application is the Wind Monitoring software that Wind Energy farms use to monitor their equipment. At the end of each day, the Wind Collector sends a message that contains all of the days statistics in JSON format which needs to be read, processed, and posted to the database. Which Azure Service is best for processing this type of data?
- a. Storage Queues
- b. Event Hub
- c. Service Bus
- d. IoT Hub

---

15. Which feature of Azure functions allow you to use a runtime not currently supported natively by Azure?
- a. Custom Handlers
- b. Durable Functions
- c. Serverless Functions
- d. SignalR

---

16. Which Azure service allows you to extend Azure File Shares from the cloud to on-premises by creating a local cache of the files?
- a. Azure AD Connect
- b. azcopy
- c. Azure Service Bus
- d. Azure File Sync

---

17. Which Azure service provides the ability to store and manage your private Docker container images?
- a. Azure Container Registry (ACR)
- b. Azure Container Instances
- c. Azure Web Apps for Containers
- d. Azure Kubernetes Service

---

18. For Windows App Services, where can you choose to have logging saved to?
- a. File system only
- b. File system, blob storage, and SQL Database
- c. File system, blob storage, and Windows Event Log
- d. File system, and blob storage

---

19. Which Durable Functions application pattern would you use for an Azure Function that only needs to run whenever an external API returns a status change?
- a. Async HTTP API
- b. Monitor pattern
- c. Fan-out/fan-in
- d. Function chaining

---

20. Which of the following statements describes the type of data that can be retrieved using Microsoft Graph?
- a. Document data, such as JSON or XML
- b. All of your Azure resources and resource groups, including deployment history and activity logs
- c. All of the data contained in Microsoft 365, including documents, calendar, email, Teams, and people.
- d. Columnar data, such as a spreadsheet or relational data table

---

21. When deploying an Azure Storage account, and you choose Zone Redundant Storage (ZRS), how many copies of your data does Azure keep?
- a. 3
- b. 1
- c. 3 copies in each Availability Zone
- d. 6

---

22. What advantage does a Spot VM provide over a regularly-provisioned VM?
- a. Spot instances are specialized virtual machines available with single, multiple, or fractional GPUs.
- b. Provides burstable performance, ideal for workloads that do not need the full performance of the CPU continuously
- c. Spot instances have a high CPU-to-memory ratio.
- d. Spot instances are significantly cheaper

--- 

23. How many input bindings is an Azure Function allowed to have?
- a. Any number or zero
- b. 0 or 1
- c. 1 or more
- d. 1

---

24. You have a docker image in your local repository that you'd like to share with the Azure Container Register. Your local repository image is named myimage, and your ACR is named myacr.azurecr.io. What is the command to get the image from your local into ACR?
- a. docker build myacr.azurecr.io/myimage
- b. docker push azurecr.io/myacr/myimage
- c. docker save myimage
- d. docker push myacr.azurecr.io/myimage

---


25. Which ASP.NET method outputs log messages to the application diagnostics log?
- a. EventLog.WriteEntry("EventSource", "message");
- b. System.Diagnostics.Trace.TraceError("message");
- c. System.Diagnostics.Debug.WriteLine("message");
- d. Console.Writeline("message")

---

26. You have a Timer Trigger Function that uses "0 15,30,45 0 * * *" as it's timer setting. How often will the function run?
- a. Every 15 minutes, every hour of the day
- b. Every 15 seconds, every minute of the day
- c. At 00:15, 00:30, and 00:45 (12:15am, 12:30am, and 12:45am); three times per day only.
- d. At 15 minutes, 30 minutes, and 45 minutes past every hour of the day

---

27. You need to modify an ARM template. You would like the location of the Azure resources to be in the same region as the resource group itself. Which ARM template function meets the criteria?

- a. `[parameters('location')]`
- b. `[environment()]`
- c. `[resourceGroup().location]`
- d. `[subscription().location]`

---

28. If your Azure solution relies on third-party public images, some risks are added to your process. Microsoft recommends keeping a private copy of public images and deploying from there, instead of deploying directly from public image locations like DockerHub. Which CLI command is able to copy a public image into Azure Container Registry?
- a. az acr import
- b. az acr copy
- c. git clone
- d. docker compose

---

29. The speed of an Azure Event Hub is determined by the number of Throughput units you reserve for it. You can set between 1 and 20 throughput units for the Event Hub. How fast does 1 throughput unit represent for data coming in to an Event Hub?
- a. 1 GB per second
- b. 1 throughput unit is one event per second
- c. 1 MB per second or 1000 events per second (whichever comes first)
- d. 1000 events per second

---

30. You are a developer for Acme Inc. You have implemented Redis as a caching service, and it's going great. You are running on a premium plan and using the top 120 GB of memory cache. You'd like to increase the memory limit to 500 GB, but Redis does not support that. How can you get more memory when using Azure Redis? Choose the best answer.
- a. Create a second Redis server and modify your application to shard your storage between the two locations.
- b. Implement the Redis Cluster feature, and add a second shard to double the memory available.
- c. Implement the Redis auto-scaling feature to automatically add and remove Redis nodes when demand exceeds 120 GB.
- d. If you attempt to store more than 120 GB of data in the memory cache, you're probably doing something wrong. Best to use an Azure SQL Database for that.