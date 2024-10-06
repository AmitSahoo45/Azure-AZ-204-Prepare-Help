### Questions

1. Which type of data can most benefit from being stored in a caching system like Azure Redis Cache?
a. Data that is called once in a session and never needed again (like a user password)
b. Data that is constantly changing
c. Data that remains relatively static
d. Data that is written and never read (like a log file)

---

2. Once you enable App Service Logging in the Azure Portal, how long does Azure keep it on?
a. 12 hours
b. 2 hours
c. Until you disable it
d. 24 hours

---

3. Generally speaking, regardless of which region, which is the lowest cost redundancy option for Blob Storage?
a. ZRS
b. LRS
c. GRS
d. GZRS

---

4. What is the Azure CLI command to create an Azure Container Instance? Fill in the blank. az ______________ --resource-group myResourceGroup --name mycontainer --image mcr.microsoft.com/azuredocs/aci-helloworld --dns-name-label aci-demo --ports 80
a. aci create
b. create container
c. container aci
d. container create

---

5. If you want to use nested ARM templates - have one ARM template include the contents of another template in it's deployment, what resource type do you use?
a. Microsoft.Resources/deploymentScripts
b. Microsoft.Resources/deployments
c. Microsoft.Compute/virtualMachines/extensions
d. "dependsOn": [ ... ]

---

6. Your company uses Azure API Management as the public front-end to its APIs, to control access. You'd like to implement certificate authentication to ensure that only authorized clients are calling the API. In which policy section do you add the ```<authentication-certificate>``` policy?
a. Backend
b. Inbound
c. Outbound
d. On-Error

---

7. What is the URL for the Azure App Service Kudu companion app?
a. https://(app-name).scm.azurewebsites.net
b. ftp://(app-name).azurewebsites.net
c. https://(app-name).kudu.azurewebsites.net
d. https://(app-name).azurewebsites.net

---

8. You have an App Service with several instances. You notice the setting ARR Affinity is enabled on the General Settings page. What does ARR Affinity do when enabled?
a. Ensure that the client is always routed to the same instance for the life of the session.
b. Optional command-line arguments for the script processor.
c. Keeps the app loaded even when there's no traffic.
d. Require client certificates in mutual authentication.

---

9. Your Azure Web App is currently throwing a 500 server error when viewed. You'd like to see more detail on the error. In order to accomplish this, what app setting do you need to set, and to what value?
a. ENVIRONMENT="Development"
b. ASPNETCORE_ENVIRONMENT="Development"
c. LOGGING="DEBUG"
d. DEBUG="TRUE"

---

10. What advantage does the Compute-Optimized (Fsv2) instance family have over the General Purpose (Dsv4) instance family?
a. F-series VMs are budget series, being much cheaper than D-series VMs
b. F-series VMs provide higher performance (ACU) per virtual CPU compared to D-series
c. They provide more temporary disk space than D-series VMs
d. F-series VMs allow you to scale to much more powerful machine sizes than D-series

---

11. Azure App Service has options to scale up and scale out. What does scaling up an app do?
a. It moves your App Service plan to a higher pricing tier, giving you more CPU, memory, disk space and extra features.
b. Switches the VM type your App Service runs on, to one with more vCPUs and more memory.
c. Increases the number of VM instances that run your app.
d. Deploys another instance of your app to a different region to ensure better performance for global customers.

---

12. Which Azure Architecture pattern is specifically designed to increase application performance using a cache service?
a. Cache-aside pattern
b. Sharding pattern
c. Static content hosting pattern
d. Sidecar pattern

---

13. Azure App Service has options to scale up and scale out. What does scaling out an app do?
a. Deploys another instance of your app to a different region to ensure better performance for global customers.
b. Adds additional running versions of your app to the same instance.
c. Increases the number of VM instances that run your app.
d. Moves to the next higher App Service Plan, such as going from S1 Standard plan to S2 Standard plan.

---

14. Your function uses the following code. You want to add a message to the log when the function starts late. What code belongs in the missing line? `[FunctionName("TimerTriggerCSharp")]` public static void Run([TimerTrigger("0 */5 * * * *")]TimerInfo myTimer, ILogger log) { >>>>> LINE MISSING HERE <<<<< { log.LogInformation("Timer is running late!"); } log.LogInformation($"C# Timer trigger function executed at: {DateTime.Now}");}
a. if (myTimer.IsPastDue)
b. if (myTimer.TriggerTime < DateTime.Now)
c. if (myTimer.IsLate)
d. if (TimerTrigger.IsLate)

---

15. In ASP.NET, how do you write a message to the application diagnostics log that only shows up when the user has enabled verbose level messages?
a. Trace.WriteLine("message");
b. Trace.TraceInformation("message");
c. Console.WriteLine("message");
d. Trace.TraceWarning("message");

---

16. How can you create a shared access signature and modify the expiry date and time after it's already been created?
a. You can edit the Shared Access Signature after it's been created in the SAS blade of the Storage Account
b. You cannot modify the expiry date of a shared access signature in any way
c. Create the shared access signature using a stored access policy
d. The only way to modify a Shared Access Signature is to recreate it

---

17. You've created a Cosmos DB account named Account1. Inside, you create one database named Db1, and one container named Container1. The data you are storing is document data using the Core (SQL) API. You have a new requirement to add a graph database using the Gremlin API. Can you create another database named Db2 inside Account1 for the graph data?
a. Yes, you can use any API to call a Cosmos DB database of any type
b. No, each account can only contain one type of data
c. Yes, each database can use a different API in one account

---

18. What is the Azure CLI command to do live streaming of application log files?
a. az webapp download
b. Get-AzAppServiceLog
c. az webapp log -all
d. az webapp log tail

---

19. What Azure Functions library do you need to implement in order for Functions to be able to call other Functions?
a. Premium Tier Functions
b. Durable functions
c. Core Tools
d. Extension Bundles

---

20. What type of App Service log files store the web server logs?
a. AppServiceAuditLogs
b. AppServiceHTTPLogs
c. AllMetrics
d. AppServiceAppLogs

---

21. How many triggers can an Azure Function have?
a. Exactly one
b. 32 maximum
c. Any number
d. 0 or 1

---

22. When creating a Cosmos DB account, you indicate which consistency level you would like to follow: Strong, Bounded Staleness, Session, Consistent Prefix and Eventual. How can a developer force Strong consistency on a query when the database itself is Eventual consistency?
a. By specifying the exact partition key and row key in the query.
b. Set the ConsistencyLevel property of QueryRequestOptions when making the query.
c. Modify the Consistency level of the database using settings before making the query.
d. Set the MaxConcurrency property of QueryRequestOptions when making the query.

---

23. You have five applications installed on a single App Service Plan. Each application has two deployment slots - production and staging. You have scaled the plan out to three instances. How many VMs are running to support this?
a. Five
b. Three
c. One
d. Ten

---

24. A Kubernetes cluster is dividend into which two components?
a. Pods, nodes
b. Control plane, Nodes
c. Containers, Container groups
d. Nodes, node pools

---

25. What does the Azure Container Registry endpoint look like?
a. azurecr.io/myprivateacr
b. myprivateacr.eastus.azurecr.io
c. myprivateacr.azurecr.io
d. registry.azure.com

---

26. You have a Timer Trigger Function that uses "0 5 * * * *" as it's timer setting. How often will the function run?
a. Once every day, at 5:00 AM
b. That's an invalid expression and the function will not run
c. Once every hour of the day, at 5 minutes after the hour
d. Every 5 minutes, every hour of the day

---

27. You have a Python app running in an Azure App Service and need to ensure that it is running on Python 3.10. Where in the Azure Portal do you set the Python version for an App Service?
a. App Service Plan > Apps
b. Configuration > General Settings
c. Settings > Properties
d. Deployment > Deployment Center

---

28. What is the concept of strong consistency with Cosmos DB?
a. With strong consistency, you are committing to use Cosmos DB in only one way in the future and forgoing other data storage models and APIs.
b. Strong consistency means that, if two data writers were to try to update the data in a Cosmos DB container, the one who updated it last would win.
c. Strong consistency is that, across the world, readers are guaranteed to always get the most recent committed version of an item.
d. Strong consistency means that, across the world, two applications might read a data item from a Cosmos DB container at the same time and get different results.

---

29. Which Azure technology allows you to implement infrastructure as code?
a. Visual Studio Enterprise Edition
b. Azure Automation Accounts
c. ARM Templates
d. GitHub Actions

---

30. You have an Azure App Service, with a WebJob. The WebJob is supposed to run continuously, but sometimes stops running as the App Service is unloaded when there are not enough incoming visitors. What can you do to ensure the App Service is never unloaded?
a. Upgrade to Standard Service Plan
b. Enable Always On setting on the General Settings page.
c. Upgrade to Premium Service Plan
d. Set the Managed Pipeline version to Integrated