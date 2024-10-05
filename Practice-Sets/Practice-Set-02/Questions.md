### Questions

Question 1: When deploying an Azure Storage account, and you choose Geo Redundant Storage (GRS), how many copies of your data does Azure keep?

- a. 3
- b. 6
- c. 2
- d. 1

---

Question 2: In ASP.NET Core, using the logger factory class, how do you write a message to the application diagnostics log that only shows up with the user has enabled warning level messages?
- a. logger.LogCritical("Message");
- b. logger.LogWarning("message");
- c. logger.LogDebug("Message");
- d. logger.LogError("Message");

---

Question 3: What is an App Service Plan?
- a. A container running inside a VM.
- b. A serverless environment in which App Services and Functions can run.
- c. An isolated physical environment including network available to your applications and no other Azure customer.
- d. A set of compute resources for a web app to run.

---

Question 4: You have a new project coming up and the development team would like to use Go as the programming language. At least some of the new project needs to be handled by Azure Functions. Go is not a native language supported by Functions. What is a feature of Azure Functions that you can use to implement Go code?
- a. Custom Handlers
- b. Durable Functions
- c. Function Orchestration
- d. Premium Functions

---

Question 5: For Azure Functions, what are the possible values for the direction property in the function.json file?
- a. blob, files, queue, table
- b. in, out, inout
- c. stderr, stdout, stdin
- d. left, right

---

Question 6: Which feature within Azure collects all of the logs from various resources into a central dashboard, where you can run queries, view graphs, and create alerts on certain events?
- a. Azure Portal Dashboard
- b. Azure Security Center
- c. Storage Account or Event Hub
- d. Azure Monitor

---

Question 7: In ASP.NET, how do you write a message to the application diagnostics log that only shows up when the user has enabled warning level messages?
- a. Console.WriteLine("message");
- b. Trace.TraceWarning("message");
- c. Trace.WriteLine("message");
- d. Trace.TraceInformation("message");

---

Question 8: What does the PowerShell command 'Get-AzVMImageSku -Location "EastUS" -PublisherName "MicrosoftWindowsServer" -Offer "WindowsServer"' return?
- a. A list of publicly available Windows Server OS images in the EastUS region.
- b. A list of available custom VM images in your Shared Image Gallery
- c. A list of running virtual machines on your subscription

---

Question 9: What type of storage container is specifically used to collect log and metric data from various Azure Resources so that it can be analyzed in Azure Monitor?
- a. Managed Storage
- b. Append Blob Storage
- c. Azure Monitor account
- d. Log Analytics Workspace

---

Question 10: What can you do to ensure your Azure Redis Cache removes keys proactively instead of waiting until memory is full?
Store the time of last access alongside the key-values, and periodically remove keys that you consider old
- a. Store the time of last access alongside the key-values, and periodically remove keys that you consider old
- b. Periodically clear the entire cache
- c. Set a low maximum cache size
- d. Set an expiration value on your keys

---

Question 11: Which library allows you to develop and test Azure Functions locally before deploying into Azure?
- a. Azure Functions compile natively to an EXE and can be run from the command line
- b. Core Tools, cross-platform on Windows, macOS and Linux
- c. Azure SDK library
- d. Azure Functions are cloud only, and cannot be tested locally

---

Question 12: You are a developer for Acme Inc. Your application uses a Service Bus Queue to receive messages from an outside app, and you have a number of applications processing those messages. You have recently been told that the business is seeing a problem with some messages in an unusual circumstance being processed twice. When you debug the problem, it's a message that was successfully processed by the job, but then the program fails before the queue could be updated to delete the message. Your boss wants you to fix the problem so that it might be better if a message was missed than if it was processed twice. What do you do to ensure messages do not get processed twice, even if sometimes they don't get processed?
- a. Implement additional error-checking code around the processing of messages so that a developer will be sent a text message whenever a message fails to process.
- b. Use only a single message processing application and this problem should go away
- c. Store the sequence number of the message in a database table at the end of the message processing task, and modify the message processing tasks to check the table before proceeding.
- d. Switch the queue to "at-most-once" delivery

---

Question 13: You are a developer for Acme Inc. You are deploying an Azure App Service, and would like to store the application secrets in Azure Key Vault. You would not like to store any user id/passwords at all inside your application. Using what method can you assign the application the permission to read the secrets from the vault, without having to store any type of authentication credentials in code?
- a. TLS mutual authentication
- b. TLS/SSL Certificate
- c. System-assigned Managed Identity, User-Assigned Managed Identity
- d. Private Link

---

Question 14: You have a Timer Trigger Function that uses "0 */5 * * * *" as it's timer setting. How often will the function run?
- a. Every 20 minutes
- b. Every 5 minutes
- c. Every 12 minutes
- d. Every 5 hours

---

Question 15: Which ASP.NET language is cross-platform and can run on both Windows and Linux Web Apps?
- a. Python
- b. Ruby
- c. ASP.NET 4
- d. ASP.NET Core

---

Question 16: You have a Timer Trigger Function that uses "0 0 0 1 1 *" as it's timer setting. How often will the function run?
- a. Every Monday at 1:00 AM
- b. At 1:01 AM every day
- c. At 12:01 AM every day
- d. At midnight on Jan 1st only

---

Question 17: Why would someone prefer a Consumption-based pricing model as opposed to a Time-based pricing model?
- a. It is always cheaper to pay for consumption than to pay by the hour
- b. You can easily predict the cost of the service into the future
- c. You can save a lot of money if you don't use the resource often as opposed to having it available for use 24/7
- d. The pricing model is simpler and easier to understand

---

Question 18: What is the maximum storage capacity of a Cosmos DB container?
- a. Unlimited
- b. 500 GB
- c. 100 GB
- d. 2 PB

--- 

Question 19: What container image formats does Azure Container Registry support?
- a. Docker images only
- b. ZIP file format
- c. Docker images, OCI images, OCI artifacts, Helm charts
- d. ISO image format

---

Question 20: For Linux App Services, where can you choose to have logging saved to?
- a. File system, blob storage, and Azure Event Hub
- b. File system, and blob storage
- c. File system only

---

Question 21: What is it that makes a caching system like Redis Cache faster than a traditional data store like Azure SQL Database?
- a. The Redis service runs on the same physical hardware as your application
- b. Stores data in memory
- c. Uses premium solid state disks
- d. Runs on the most powerful servers

---

Question 22: ARM templates are said to have a declarative syntax. Why is a declarative syntax better than a programmatic approach?
- a. Declarative syntax supports advanced techniques such as looping, variables, parameters and random resource names
- b. Declarative syntax supports code source control such as Github
- c. Declarative syntax only requires minor changes to the code before each deployment to ensure uniqueness
- d. You don't need to worry about the order of operations to create resources (dependencies), Azure takes care of creating them in the correct order

---

Question 23: You have an Azure Container Instance with the DNS label "mycontainer". What is the public Fully-Qualified Domain Name (FQDN) for that instance?
- a. mycontainer.azurecontainer.io
- b. mycontainer.(azureregion).azurecontainer.io
- c. azurecontainer.io/mycontainer
- d. mycontainer.container.azure.com

---

Question 24: When writing code that connects to an Azure Storage account, you set the Retry option mode to Exponential. What does Exponential mode do?
- a. Retry attempts will delay based on a backoff strategy, where each attempt will increase the duration that it waits before retrying.
- b. Retry attempts happen at fixed intervals; each delay is a consistent duration

---

Question 25: All Azure data resources (Cosmos DB, SQL Database, Redis Cache, etc) must belong to one and only one.... ?
- a. Resource Group
- b. Virtual Network
- c. Availability Zone
- d. Azure AD Group

---

Question 26: What is the major downside/risk to using Spot VMs compared to regularly-provisioned VMs?
- a. They can cost more than a regularly-provisioned VM
- b. Eviction
- c. There is no SLA
- d. You are limited to how many spot instances you can have

---

Question 27: Which CosmosDB API format works best with graph data?
- a. Table API
- b. Cassandra API
- c. Core (SQL) API
- d. Gremlin API

---

Question 28: Which of the following Azure CLI commands is considered part of the ACR Tasks set?
- a. az acr build
- b. az acr update
- c. az acr create
- d. az acr import

---

Question 29: Which Azure CLI command will create a container image of your code and automatically deploy to Azure Container Registry?
- a. az acr create
- b. az acr build
- c. docker push
- d. docker compose up

---

Question 30: When a Virtual Machine named VM1 is deployed to a virtual network named Vnet1, and a subnet named Subnet1, which private IP address is it given?
- a. The first available private IP address in the Subnet1 address range
- b. 10.0.0.2 is always the first IP given to a VM on a new VNet
- c. A random and unknowable IP address
- d. An IP from Azure's large pool of public IP addresses

