### Answer Key

1. b. The cold start problem

Explanation: Azure Functions Broadly speaking, the cold start problem is a term used to describe the phenomenon that applications that haven’t been used take longer to start up. In the context of Azure Functions, latency is the total time a user must wait for their function. From when an event happens to start up a function until that function completes responding to the event. So more precisely, a cold start is an increase in latency for Functions that haven’t been called recently. When using Azure Functions in the dedicated plan, the Functions host is always running, which means that cold start isn’t really an issue. So, our scope is narrowed to Functions running the serverless consumption model.

Refer to the Microsoft Doc: https://azure.microsoft.com/en-us/blog/understanding-serverless-cold-start/

---

2. d. retention

Explanation: Azure Container Registry allows you to set a retention policy for stored image manifests that don't have any associated tags (untagged manifests). When a retention policy is enabled, untagged manifests in the registry are automatically deleted after the number of days you set. This feature prevents the registry from filling up with artifacts that aren't needed and helps you save on storage costs.  The retention keyword sets the retention policy. 

Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-registry/container-registry-retention-policy

---

3. b. Authenticator app, text message, phone call, security key

Explanation: Only the following methods can be used for two-factor verification: Authenticator app, text message, phone call, security key Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/active-directory/user-help/security-info-setup-email

---

4. c. The Connection Strings tab of the App Service configuration

Explanation: For ASP.NET and ASP.NET Core developers, setting connection strings in App Service are like setting them in `<connectionStrings>` in Web.config, but the values you set in App Service override the ones in Web.config. You can keep development settings (for example, a database file) in Web.config and production secrets (for example, SQL Database credentials) safely in App Service. The same code uses your development settings when you debug locally, and it uses your production secrets when deployed to Azure. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/configure-common#configure-connection-strings

---

5. d. Kudu

Explanation: Kudu is the engine behind a number of features in Azure App Service related to source control based deployment, and other deployment methods like Dropbox and OneDrive sync. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/resources-kudu

---

6. d. Azure Key Vault

Explanation: Azure Key Vault - the modern way to store cryptographic keys, signed certificates and secrets in AzureFor more info: <a href='https://docs.microsoft.com/en-us/azure/key-vault/'>https://docs.microsoft.com/en-us/azure/key-vault/</a>

---

7. b. Table API

Explanation: Table API stores data in key/value format. Gremlin API allows users to make graph queries and stores data as edges and vertices. Cassandra API stores data in column-oriented schema. MongoDB API stores data in a document structure, via BSON format. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/cosmos-db/introduction

---

8. b. Point-in-time restore

Explanation: Point-in-time restore protects against accidental deletion or corruption by enabling you to restore block blob data to an earlier state. Point-in-time restore is useful when a user or application accidentally deletes data or an application error corrupts data. Point-in-time restore also enables testing scenarios that require reverting a data set to a known state before running further tests.  Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/storage/blobs/point-in-time-restore-overview

---

9. c. Two

Explanation: When you create an app in App Service, it is put into an App Service plan. When the app runs, it runs on all the VM instances configured in the App Service plan. If multiple apps are in the same App Service plan, they all share the same VM instances. If you have multiple deployment slots for an app, all deployment slots also run on the same VM instances. In this way, the App Service plan is the scale unit of the App Service apps. If the plan is configured to run five VM instances, then all apps in the plan run on all five instances. If the plan is configured for autoscaling, then all apps in the plan are scaled out together based on the autoscale settings. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/overview-hosting-plans

---

10. b. False

Explanation: You cannot get an Azure Function to trigger off an incoming email.

---

11. c. container delete

Explanation: azure container delete will delete a running container instance. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-instances/container-instances-quickstart

---

12. d. CLI, PowerShell, Portal, Visual Studio Code, ARM Template

Explanation: You can create resources using all REST channels (Portal, PowerShell, CLI, ARM Templates) plus using the Visual Code Extension. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/api-management/vscode-create-service-instance

---

13. a. AzCopy

Explanation: AzCopy is the tool that can be used to copy large amounts of files between storage containers and accounts.

---

14. d. Inserts and updates

Explanation: Today, you see all inserts and updates in the change feed. You can't filter the change feed for a specific type of operation. One possible alternative is to add a "soft marker" on the item for updates and filter based on that when processing items in the change feed. Currently, the change feed doesn't log deletes. Similar to the previous example, you can add a soft marker on the items that are being deleted. For example, you can add an attribute in the item called "deleted" and set it to "true" and set a TTL on the item so that it can be automatically deleted.  You can read the change feed as far back as the origin of your container, but if an item is deleted, it will be removed from the change feed. 

---

15. c. YAML file

Explanation: Docker containers use YAML files for configuration settings. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-instances/tutorial-docker-compose

---

16. d. Region, pricing tier, hours

Explanation: Redis Cache is charged by the hour, and varies by region. It also depends on the tier you choose. Refer to Microsoft Doc: https://azure.microsoft.com/en-us/pricing/details/cache/

---

17. b. Windows, Linux and macOS

Explanation: Azure Files offers fully managed file shares in the cloud that are accessible via the industry standard Server Message Block (SMB) protocol or Network File System (NFS) protocol. Azure file shares can be mounted concurrently by cloud or on-premises deployments. Azure Files SMB file shares are accessible from Windows, Linux, and macOS clients. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/storage/files/storage-files-introduction

---

18. b. Settings > Container > Logs

Explanation: Viewing the logs for a container instance is helpful when troubleshooting issues with your container or the application it runs. To view the container's logs, under Settings, select Containers, then Logs. You should see the HTTP GET request generated when you viewed the application in your browser. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/container-instances/container-instances-quickstart-portal

---

19. c. ARM templates

Explanation: ARM templates are a way of defining your infrastructure using declaritive statements, as opposed to scripts. You define what you want your resources to look like, including the properties and values, and Azure will ensure they look that way. Scripts suffer from the problem of not being able to run the same script twice, whereas ARM templates can be deployed again and again without issue. This is sometimes called Desired State Configuration (or DSC). Refer to Microsoft Doc: https://docs.microsoft.com/en-us/learn/modules/explore-provision-deploy-non-relational-data-services-azure/2-describe-provision-non-relational-data-services

---

20. b. Cross-Origin Resource Sharing (CORS)

Explanation: Cross Origin Resource Sharing (CORS) is a standard with web browsers that will prevent a website from calling an API in the browser unless the API explicitly allows the call.

---

21. c. Serverless

Explanation: Azure Container Instances are on-demand containers in a managed, serverless Azure environment. Azure Container Instances is a solution for any scenario that can operate in isolated containers, without orchestration. Run event-driven applications, quickly deploy from your container development pipelines, and run data processing and build jobs. Refer to Microsoft Doc: https://docs.microsoft.com/bs-cyrl-ba/azure/container-instances/

---

22. a. Core Tools, cross-platform on Windows, macOS and Linux

Explanation: Azure Functions Core Tools provides the core runtime and templates for creating functions, which enable local development. Version 2.X supports development on Windows, Linux, and MacOS. 

Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-functions/functions-develop-local

---

23. d. Soft Delete

Explanation: Soft Delete allows you to recover deleted files within a set time period as configured. Change Feed would not allow you to recover deleted files. Immutable blobs can restrict deletion but not help you recover files. And Azure Policy does not have an option that deals with the contents of a storage account. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/learn/modules/explore-non-relational-data-offerings-azure/3-explore-azure-blob-storage

---

24. a. You cannot. If you want to move an app between regions, you must clone the app, or redeploy the app from scratch.

Explanation: You can move an app to another App Service plan as long as the source plan and the target plan are in the same resource group and geographical region. The region in which your app runs is the region of the App Service plan it's in. However, you cannot change an App Service plan's region. If you want to run your app in a different region, one alternative is app cloning. Cloning copies your app in a new or existing App Service plan in any region. 

Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/app-service/app-service-plan-manage

---

25. c. It outputs a sorted list of documents that were changed in the order in which they were modified.

Explanation: Change feed in Azure Cosmos DB is a persistent record of changes to a container in the order they occur. Change feed support in Azure Cosmos DB works by listening to an Azure Cosmos container for any changes. It then outputs the sorted list of documents that were changed in the order in which they were modified. The persisted changes can be processed asynchronously and incrementally, and the output can be distributed across one or more consumers for parallel processing. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/cosmos-db/change-feed

---

26. a. 3

Explanation: Azure Storage always stores multiple copies of your data so that it is protected from planned and unplanned events, including transient hardware failures, network or power outages, and massive natural disasters. Redundancy ensures that your storage account meets its availability and durability targets even in the face of failures. Locally redundant storage (LRS) copies your data synchronously three times within a single physical location in the primary region. LRS is the least expensive replication option, but is not recommended for applications requiring high availability or durability. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/storage/common/storage-redundancy

---

27. d. Docker YAML file

Explanation: Both a parameters and template json files are downloaded.  Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/quickstart-create-templates-use-the-portal

---

28. c. Web App for Containers is much easier to deploy and control than a Kubernetes cluster

Explanation: Web App for Containers is much easier to deploy and control than a Kubernetes cluster. You get a lot of the developer-friendly features of Azure App Services, and avoid having to start and control clusters of computers. Refer to Microsoft Doc: https://azure.microsoft.com/en-ca/blog/webapp-for-containers-overview/

---

29. b. Your app pulls the secret from Key Vault (using App Configuration) and not hard-coded in the app.config file.

Explanation: Using App Configuration to connect to Key Vault will allow you to continue to use App Configuration commands in your app, but the secrets are pulled from Key Vault securely. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-app-configuration/use-key-vault-references-dotnet-core?tabs=core5x

---

30. d. PUT /api/zip/{path}/

Explanation: The Zip API allows downloading folders as zip files, or expanding zip files into folders. Refer to Microsoft Doc: https://github.com/projectkudu/kudu/wiki/REST-API
