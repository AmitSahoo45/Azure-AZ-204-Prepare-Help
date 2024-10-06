### Question

1. Which of the following is a negative consequence of running Azure Functions in the Consumption service plan?

- a. It's the most expensive way to run Functions
- b. The cold start problem
- c. Functions can only be developed inside the Portal and not locally
- d. Performance is not as good as an App Service Plan

---

2. Your Azure Container Registry is getting quite big. You have to find a way to reduce the size of it by removing unused images. You decided to delete any untagged images after 30 days. Which Azure CLI command is used automatically remove untagged images? Fill in the blank.  az acr config ________ update --registry myregistry --status enabled --days 30 --type UntaggedManifests
- a. timeout
- b. untagged
- c. delete
- d. retention

---

3. Which of the following two-factor authentication verification methods are available in Azure AD?
- a. Email, SMS, Security Questions
- b. Authenticator app, text message, phone call, security key
- c . Text message
- d. Authenticator App, text message, email, phone call

---

4. You are developer encountering an issue with your Azure App Service web app. The app appears to be failing to connect to the database. You notice that the connection string appears both in the `<connectionStrings>` section of web.config AND ALSO appears in the Connection Strings tab of the App Service configuration. Which database connection string is being used by the application in production?
- a. The Connection String in the web.config
- b. There's no way to know why connection string will be chosen
- c. The Connection Strings tab of the App Service configuration

---

5. What is the engine behind Azure App Service source control based deployment, and other deployment methods like ZIP file upload?
- a. Migration Assistant
- b. REST API
- c. Azure Portal
- d. Kudu

---

6. What is the recommended way within Azure to store secrets such as private cryptographic keys?
- a. Within the application code
- b. Azure Advanced Threat Protection (ATP)
- c. In an Azure Storage account private blob container
- d. Azure Key Vault

---

7. Which CosmosDB API format works best with key-value data?
- a. MongoDB API
- b. Table API
- c. Cassandra API
- d. Gremlin API

---

8. Which feature of Azure Storage Account allows you to restore one or more containers to an earlier state?
- a. Soft delete for containers
- b. Point-in-time restore
- c. Soft delete
- d. Azure Backup

---

9. You have one application installed in an App Service Plan Standard S1 Tier. You have manually scaled it out to two instances. This application also has one WebJob running in the background to support it. How many VMs are running to support this?
- a. Three
- b. One
- c. Two
- d. Four

---

10. True or false: you can create an Azure Function to run whenever a new email comes into Outlook using it's own native Trigger integration with email
- a. TRUE
- b. FALSE

---

11. What is the Azure CLI command to delete an Azure Container Instance? Fill in the blank. az ______ _______ --resource-group myResourceGroup --name mycontainer
- a. delete resource
- b. aci delete
- c. container delete
- d. delete container

---

12. Using which channels can you create an API Management instance?
- a. Portal only
- b. CLI, PowerShell, Portal
- c. Portal, ARM Template
- d. CLI, PowerShell, Portal, Visual Studio Code, ARM Template

---

13. What Azure command line tool for Windows and Linux is designed to copy data to and from a Blob storage account, across containers, and across storage accounts?
- a. AzCopy
- b. xcopy
- c. bcp
- d. Azure Storage Explorer

---

14. Which types of database changes does the CosmosDB change feed track?
- a. Inserts only
- b. Updates only
- c. Inserts, updates and deletes
- d. Inserts and updates

---

15. Which file format is the standard for documenting the configuration of Docker containers and is used by Docker Compose to create the image?
- a. .config file
- b. XML file
- c. YAML file
- d. JSON file

---

16. Which of the following metrics affect how much an Azure Redis Cache instance costs?
- a. Region, Pricing tier
- b. Region, Consumed storage, pricing tier
- c. Per transaction
- d. Region, pricing tier, hours

---

17. Which operating systems can mount an external drive using Azure File Share?
- a. Windows Only
- b. Windows, Linux and macOS
- c. Windows and Linux Only
- d. Android and iOS Only

---

18. Under which menu item of the Azure Portal can you find the logs for a container instance?
- a. Monitoring > Alerts
- b. Settings > Container > Logs
- c. Monitoring > Metrics
- d. Overview

---

19. What method of provisioning a non-relational database involves first defining the database in a JSON file, which can then be checked into a code repository for source control, sometimes also referred to as Infrastructure as Code?
- a. Azure Portal
- b. PowerShell Scripts
- c. ARM templates
- d. CLI Bash Shell

---

20. What security feature exists for API apps that will either allow or prevent applications running from other domains (external websites) from calling the API?
- a. RBAC
- b. Cross-Origin Resource Sharing (CORS)
- c. Cross Site Scripting (XSS)
- d. Azure AD

---

21. What type of compute is Azure Container Instances considered to be?
- a. Infrastructure as a Service
- b. Hybrid Compute
- c. Serverless
- d. Virtual Machine Scale Set

---

22. Which library allows you to develop and test Azure Functions locally before deploying into Azure?
- a. Core Tools, cross-platform on Windows, macOS and Linux
- b. Azure Functions compile natively to an EXE and can be run from the command line
- c. Azure Functions are cloud only, and cannot be tested locally
- d. Azure SDK library

---

23. What feature of Azure Blob Storage, if enabled, allows you to retrieve files that have previously been deleted within a time period?
- a. Change Feed
- b. Azure Policy
- c. Immutable blobs
- d. Soft Delete

---

24. You have created a web app called TestWebApp in the West US region. After creating it, you decide you'd rather this web app run in the East US region. How do you move a Web App to a new region?
- a. You cannot. If you want to move an app between regions, you must clone the app, or redeploy the app from scratch.
- b. In the Azure Portal, open the Web App, and chooose the Move menu at the top of the Overview screen
- c. You can't move the web app, but you can move the App Service Plan it runs in which has the same effect.
- d. It can only be done in PowerShell or CLI

---

25. What does the Change Feed do when configured in Azure Cosmos DB?
- a. Outputs a list of documents in the container, along with the date they were last modified
- b. Sends an alert to an Action Group (SMS, Email, Function, etc) when data changes in Cosmos DB
- c. It outputs a sorted list of documents that were changed in the order in which they were modified.
- d. Sends an alert to Azure Portal notifications when data changes in Cosmos DB

---

26. When deploying an Azure Storage account, and you choose Locally Redundant Storage (LRS), how many copies of your data does Azure keep?
- a. 3
- b. 1 copy in each Availability Zone
- c. 6
- d. 1

---

27. When you download an ARM Template from the Portal, just before confirming a deployment, what is the one file that is not downloaded to your computer?
- a. Powershell and CLI deployment scripts
- b. Parameters JSON file
- c. Template JSON file
- d. Docker YAML file

---

28. Why should a developer choose to deploy a container to a Web App for Containers instead of Azure Kubernetes Service?
- a. Web App for Containers provide much more low-level control over the scaling and performance of the app
- b. AKS is more for development and product demos, while Web App for Containers is an enterprise solution for containerized applications
- c. Web App for Containers is much easier to deploy and control than a Kubernetes cluster
- d. Web App for Containers integrates seamlessly with your other AKS containers and can be controlled with the same commands

---

29. What effect does adding a Key Vault Reference to your app using Configuration Explorer have?
- a. A Key Vault will be created for you if one does not exist
- b. Your app pulls the secret from Key Vault (using App Configuration) and not hard-coded in the app.config file.
- c. Your application will use SSL/HTTPS for communication
- d. You can connect to the key vault by code inside your application

---

30. What is the REST API command for uploading a ZIP file into an Azure App Service using the Kudu SCM endpoint?
- a. POST /api/scm/{path}/
- b. PUT /api/deployments/{id}
- c. POST /deploy
- d. PUT /api/zip/{path}/