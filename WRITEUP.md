# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- COST
VM: A Virtual Machine is more expensive because you pay for the whole server all the time, even when the app is not heavily used. You also spend extra time and effort maintaining the OS, updates, and security, which adds to the overall cost.
App Service: App Service is cheaper for small web apps because you only pay for the hosting plan and not a full machine. Since Azure manages the platform, there are no hidden costs for maintenance or system administration.
-SCALABILITY
VM: Scaling a VM requires creating new instances, configuring load balancers, and managing the capacity yourself. This takes more time and technical setup, especially if traffic increases suddenly.
App Service: App Service can scale automatically with just a few settings, and Azure handles the creation of new instances in the background. This makes it easier and faster to support more users without manual configuration.
-AVAILABILITY
VM: Keeping a VM highly available requires setting up backups, monitoring, and failover systems on your own. If the VM needs a restart or update, downtime is more likely unless additional configuration is done.
App Service: App Service provides built-in high availability since Azure manages the platform updates and infrastructure. Your app stays online more consistently without extra work from you.
-WORKFLOW 
VM: Deploying on a VM means you must manage the server, install packages, apply security patches, and manually handle deployments. This can slow down development and increases the risk of configuration errors.
App Service: App Service simplifies the workflow by supporting direct GitHub deployments and automatic updates. You don’t have to worry about server maintenance, so you can focus only on your application code.

- *Choose the appropriate solution (VM or App Service) for deploying the app*
- The appropriate solution for deploying this application is Azure App Service. It provides a managed environment designed for running web applications without the need to configure or maintain a full server. App Service also supports direct deployment from GitHub, making updates and continuous delivery much easier. It meets all the essential hosting and workflow needs of this CMS project.
- 
- *Justify your choice*
- Azure App Service is selected because it reduces the operational effort compared to using a VM. It handles platform updates, scaling, and availability automatically, allowing more focus on the application itself rather than server management. The pricing model is also more efficient for a lightweight web app that doesn’t require full OS-level control. Overall, it offers a simpler, more reliable, and more streamlined deployment setup for this project.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

My decision would shift toward using a VM only if the application required capabilities that App Service cannot support. For example, if the project needed custom background services, special OS dependencies, or software that requires direct server access, a VM would be more appropriate. In situations where full infrastructure control or highly specialized configurations are necessary, choosing a VM would make more sense than relying on the managed environment of App Service.
