# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- Cost
VM: A Virtual Machine is more expensive because you pay for the whole server all the time, even when the app is not heavily used. You also spend extra time and effort maintaining the OS, updates, and security, which adds to the overall cost.
App Service: App Service is cheaper for small web apps because you only pay for the hosting plan and not a full machine. Since Azure manages the platform, there are no hidden costs for maintenance or system administration.
Scalability
VM: Scaling a VM requires creating new instances, configuring load balancers, and managing the capacity yourself. This takes more time and technical setup, especially if traffic increases suddenly.
App Service: App Service can scale automatically with just a few settings, and Azure handles the creation of new instances in the background. This makes it easier and faster to support more users without manual configuration.
Availability
VM: Keeping a VM highly available requires setting up backups, monitoring, and failover systems on your own. If the VM needs a restart or update, downtime is more likely unless additional configuration is done.
App Service: App Service provides built-in high availability since Azure manages the platform updates and infrastructure. Your app stays online more consistently without extra work from you.
Workflow 
VM: Deploying on a VM means you must manage the server, install packages, apply security patches, and manually handle deployments. This can slow down development and increases the risk of configuration errors.
App Service: App Service simplifies the workflow by supporting direct GitHub deployments and automatic updates. You don’t have to worry about server maintenance, so you can focus only on your application code.

- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
