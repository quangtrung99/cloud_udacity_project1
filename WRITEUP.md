# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

- Analyze:
Cost: An App Service more cost effective than VMs. Pricing is based on the chosen plan (example: Free, Shared, Basic, Standard, Premium).
Scalability: VMs offer high scalability but require manual or custom scripts to scale up or down. App Service offer automatic scaling options, this make it easier to handle workload without manual intervention.
Availability: VMs have high availability because we can setup multiple VMs and load balancers, but this will add more cost and complexity. App Service provide to us built-in high availability and disaster recovery options with minimal configuration required.
Workflow: VMs provide us full control over the environment and this benefit will be greate if we want custom and install specific software for server. With App Service, It simplier deployment and management with integrate CI/CD pipeline, make it easier to maintain and update the app.

- Choose for this project solution: I will use App Service. 
- Justify My Choice: Because this is just a small project and doesn't need to install any specific software and we just need a simplier way for deploy this app. And based on an analyze above, this service is enough for me.


### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

If the project CMS requires:
- Install custom software or specific OS configuration. -> This is not support in App Service.
- Complex Networking Requirements: VMs provide more flexibility in networking configuration due to App Service. If app need advanced networking features, a VM would be better choice.
- Significant Increase in traffic: the traffic exceed the scaling capabilities of App Service plan.

