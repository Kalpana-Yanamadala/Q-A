**DevOps Interview Guide: Questions, Sample Answers & Evaluation Criteria**

---

### 🔹 Basic (Junior to Associate Level)

#### 1. Azure DevOps Fundamentals

**Q:** What is Azure DevOps and what services does it include?
**A:** Azure DevOps is a suite of development tools for software teams. It includes services like Azure Repos, Azure Pipelines, Azure Boards, Azure Artifacts, and Azure Test Plans.
**Evaluation:** Understanding of DevOps as a platform, ability to name core services.

**Q:** How do you set up a basic CI/CD pipeline in Azure DevOps?
**A:** Use Azure Pipelines to define CI/CD in YAML. Connect to a Git repo, define build tasks, add stages for deployment.
**Evaluation:** Familiarity with build/release stages, basic YAML syntax.

#### 2. Scripting & Automation Basics

**Q:** Can you write a simple PowerShell script to stop/start an Azure VM?
**A:** `Stop-AzVM -Name "myVM" -ResourceGroupName "myRG"`
**Evaluation:** Basic syntax knowledge and usage of Az PowerShell module.

#### 3. Cloud Concepts

**Q:** What is a Resource Group in Azure?
**A:** A container that holds related resources like VMs, databases, and web apps.
**Evaluation:** Basic understanding of resource management in Azure.

#### 4. Monitoring

**Q:** What is Application Insights used for?
**A:** Monitoring live applications, collecting telemetry data, analyzing performance.
**Evaluation:** High-level understanding of AppInsights purpose.

#### 5. Databases

**Q:** What's the difference between SQL Server and Oracle in Azure?
**A:** SQL Server is a Microsoft product with full integration in Azure. Oracle is supported via IaaS or Marketplace solutions.
**Evaluation:** Basic DB platform understanding.

---

### 🔸 Intermediate (Mid-Level)

#### 6. Azure DevOps & CI/CD

**Q:** How do you manage secrets in Azure DevOps?
**A:** Use Azure Key Vault and link it to pipeline variables.
**Evaluation:** Knowledge of secure DevOps practices.

**Q:** Explain pipeline templates.
**A:** YAML templates help reuse CI/CD logic across multiple pipelines, promoting DRY principles.
**Evaluation:** Reusability and code organization skills.

#### 7. IaC (Terraform/ARM)

**Q:** How would you modularize Terraform code?
**A:** Split resources into modules (network, compute, storage), define variables and outputs, use remote state.
**Evaluation:** Code organization and environment separation.

**Q:** Compare ARM and Terraform.
**A:** ARM is Azure-native, tightly integrated. Terraform is multi-cloud and uses HCL. Terraform offers better community support and modularity.
**Evaluation:** Depth of IaC tooling knowledge.

#### 8. Containers

**Q:** How do you containerize a .NET app?
**A:** Create Dockerfile, build image using `docker build`, run using `docker run`, push to ACR.
**Evaluation:** Hands-on Docker knowledge.

#### 9. Monitoring & Logging

**Q:** How do you visualize telemetry data in Power BI?
**A:** Connect Power BI to Azure Monitor Logs via Log Analytics API, build reports.
**Evaluation:** Ability to bridge DevOps and data visualization.

---

### 🔶 Senior-Level (Lead/Architect)

#### 10. Advanced CI/CD & Architecture

**Q:** Describe a complex CI/CD pipeline you designed.
**A:** Multi-stage pipeline with dev/test/prod stages, integrated with SonarQube, security scanning, manual approvals.
**Evaluation:** Strategic thinking, end-to-end automation knowledge.

#### 11. Cloud Strategy

**Q:** How would you migrate a workload from Azure to AWS?
**A:** Evaluate dependencies, use IaC to replicate infra, migrate data using Data Box/Migration tools, cutover with DNS switch.
**Evaluation:** Cloud agnosticism, planning skills.

#### 12. Security & Governance

**Q:** How do you enforce compliance in IaC?
**A:** Use Terraform Sentinel or Azure Policy for guardrails. Validate configs in CI pipeline.
**Evaluation:** Preventative controls and governance understanding.

#### 13. Networking

**Q:** When would you use Azure Front Door over App Gateway?
**A:** Front Door for global HTTP/HTTPS routing and WAF. App Gateway for regional traffic and internal load balancing.
**Evaluation:** Solution-oriented thinking.

#### 14. CMS & Custom Components

**Q:** How do you build and release Sitecore/Dynamics CRM components?
**A:** Use MSBuild or PowerShell to package components, deploy via Azure DevOps using agent-based or script deployments.
**Evaluation:** Integration knowledge with specialized CMS tools.

#### 15. Leadership

**Q:** How do you mentor junior engineers?
**A:** Pair programming, code reviews, brown-bag sessions, goal-setting.
**Evaluation:** People management and coaching.

#### 16. Cross-Team Collaboration

**Q:** How do you work with product/QA/architect teams?
**A:** Attend planning sessions, ensure shared definitions of done, track dependencies, prioritize DevOps tasks collaboratively.
**Evaluation:** Team alignment and communication.

---

Let me know if you'd like this exported as a PDF or converted into a quiz/study format.
