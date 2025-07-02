**1. What is DevOps and why is it important in modern software development?**
   
✅ Sample Answer:

DevOps is a set of practices that combines software development and IT operations. It aims to shorten the development lifecycle, improve collaboration, and deliver features, fixes, and updates frequently in close alignment with business objectives. DevOps is important because it promotes faster, more reliable releases through automation, continuous integration, and continuous delivery.

**2. What is Infrastructure as Code (IaC)?**
   
✅ Sample Answer:

IaC is the practice of managing and provisioning infrastructure using code instead of manual processes. Tools like Terraform or Ansible allow you to define infrastructure in version-controlled files, enabling repeatability, automation, and consistency across environments.

**3. How do you use Terraform in a real project?**
   
✅ Sample Answer:

I use Terraform to provision cloud infrastructure in Azure. For example, I’ve used it to create AKS clusters, storage accounts, and virtual networks. I separate configurations using modules and keep state in remote storage like Azure Blob Storage. We integrate Terraform into our CI/CD pipelines to ensure consistent deployments.

**4. How do you secure a CI/CD pipeline?**
   
✅ Sample Answer:

I secure pipelines by integrating static code analysis and dependency scans (e.g., SonarQube, Snyk), storing secrets securely using Azure Key Vault, and using signed artifacts. I ensure least privilege access to pipeline agents and limit who can trigger deployments. We also run vulnerability scans on Docker images and perform regular audits.

**5. How do you handle application monitoring and alerting?**
   
✅ Sample Answer:

I use tools like Splunk or New Relic for log aggregation and application performance monitoring. We set up dashboards and alerts based on error rates, latency, and resource usage. Alerts are routed to PagerDuty or Slack so teams can respond quickly. We use synthetic monitoring for uptime checks.

**6. How have you promoted DevOps culture in your previous teams?**
   
✅ Sample Answer:

I encouraged product teams to own their deployments by building reusable CI/CD templates and conducting DevOps workshops. I helped implement a “you build it, you run it” model and shifted ops responsibilities into squads by embedding automation and observability into the pipelines. I also mentored engineers in IaC and containerization.

**7. Describe a complex CI/CD pipeline you’ve built or maintained.**
   
✅ Sample Answer:

I built a CI/CD pipeline for a microservices platform hosted on AKS using GitHub Actions. Each service had its own workflow, running tests, scanning with SonarQube and Trivy, building Docker images, pushing to ACR, and deploying via Helm charts. We used branch protections and manual approvals for production deployments.

**8. How do you lead a multi-skilled DevOps/Platform team?**
   
✅ Sample Answer:

I focus on balancing technical delivery with team growth. I conduct regular 1:1s, set clear goals, encourage pair programming and knowledge sharing, and rotate responsibilities (e.g., on-call, incident response). I involve the team in architectural decisions and align with business priorities through cross-functional planning.
