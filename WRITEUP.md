# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

## For Both VM and App Service:

Costs:

- VM: Offers some potential cost savings, especially during periods of low traffic, as you only pay for the resources you use. However, managing a VM requires additional staff time, which translates to ongoing costs.
App Service: Costs are consistent, even during downtimes. However, its pricing tiers ensure efficient resource allocation, making it cost-effective for most CMS applications.

Scalability:

- VM: Offers granular control over scaling by manually adding or removing VM instances.
- App Service: Provides automatic scaling based on predefined rules or traffic patterns, simplifying resource management.

Availability:

- VM: Offers high availability (99.5% SLA) through careful configuration and redundancy strategies.
- App Service: Delivers high availability (99.95% SLA) with built-in redundancy and disaster recovery features.

Workflow:

- VM: Requires manual configuration, patching, and software installation, leading to a more complex deployment process.
- App Service: Offers a seamless workflow with continuous deployment options from platforms like GitHub, enabling faster deployments.
Choosing the Appropriate Solution:

## Based on the analysis, App Service is the most suitable solution for deploying the CMS app due to the following reasons:

- Simplicity: The straightforward nature of the CMS app and its Python codebase align well with App Service's pre-configured environment.
- Reduced Cost for Lightweight Applications: App Service pricing tiers are cost-effective for resource-efficient apps like CMS.
- Faster Deployment: Streamlined deployment through continuous integration/continuous delivery (CI/CD) with Azure DevOps or GitHub workflows minimizes deployment time.
- Justification: 
In this case, the benefits of App Service outweigh the potential cost savings of a VM. The reduced complexity, faster deployment times, and built-in management features make App Service the most efficient and cost-effective option for this specific CMS application.
 
### Assess app changes that would change your decision.
Here's how the app and other needs might change to influence the decision:

Increased Functionality: If the CMS app integrates with custom software or requires specific libraries not supported by App Service, a VM would offer the necessary control over the environment.
Security Requirements: For highly sensitive data or specialized security needs beyond App Service's offerings, a VM might provide a more customizable security posture.
Performance Demands: If the CMS app experiences significant traffic spikes or requires real-time, low-latency processing, a VM might offer more fine-grained control over hardware resources for optimal performance.
