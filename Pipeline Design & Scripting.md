❓ **1. How would you design a multi-stage pipeline for a microservices application?**

  For a microservices app, design the pipeline as modular and parallelizable, ideally with these stages:

🧱** Multi-Stage Pipeline Design:**

    Stage 1 – Build & Test (per microservice):
    
    Run independently for each service
    
    Compile code, run unit tests, linting
    
    Use Docker for image packaging
    
    Stage 2 – Integration Testing:
    
    Deploy services to a test environment (e.g., via Docker Compose or Kubernetes)
    
    Run integration and contract tests
    
    Stage 3 – Staging Deployment:
    
    Deploy to a pre-prod or staging environment
    
    Smoke and performance tests
    
    Stage 4 – Production Deployment:
    
    Approvals or gates
    
    Use blue/green or canary strategies
    
    Stage 5 – Monitoring & Rollback:
    
    Integrate logging/monitoring (e.g., Prometheus, ELK)

Enable rollback hooks on failure

Tools: GitHub Actions, GitLab CI, Azure DevOps, ArgoCD

❓ **2. What are build agents or runners, and how do they work?**

Build agents (or runners) are compute nodes that execute CI/CD pipeline jobs.

🔧 **How they work:**

    Listen for jobs from the CI server (e.g., Jenkins master, GitLab server)
    
    Pull the code from the repo
    
    Execute defined steps (build, test, deploy)
    
    Report results back to the pipeline

Types:

    Self-hosted runners (custom config, private infra)
    
    Hosted runners (provided by GitHub, Azure, etc.)

Example:

In GitHub Actions:

runs-on: ubuntu-latest tells the workflow to use GitHub's hosted runner.

❓ **3. How do you handle secrets or credentials in CI/CD pipelines?**

Handling secrets securely is critical in CI/CD:

🔐 Best Practices:

    Use secure secret management services:
    
    GitHub Actions → GitHub Secrets
    
    Azure Pipelines → Azure Key Vault + Variable Groups
    
    GitLab → CI/CD Variables
    
    Never store secrets in code or logs
    
    Rotate secrets periodically
    
    Limit access using least privilege principle
    
    Use encrypted environment variables in pipeline YAML
    
    Example (GitHub Actions):
    
env:

  DB_PASSWORD: ${{ secrets.DB_PASSWORD }}
  
❓ **4. How do you manage pipeline-as-code (YAML)?**

Pipeline-as-code means defining your pipeline in version-controlled YAML files.

📄 Benefits:

Version-controlled and peer-reviewed

Portable and reusable

Easier to track changes and rollback

🛠️** Best Practices:**

Keep it modular using templates/includes (Azure DevOps, GitLab)

Reuse logic via reusable workflows/jobs

Use variables to avoid hardcoding

Split logic per service in monorepos

Example (GitHub Actions YAML):

  jobs:
    build:
      runs-on: ubuntu-latest
      steps:
        - run: npm install
        - run: npm test
        
❓ **5. How do you implement rollback strategies in CI/CD?**

Rollback strategies are used when a deployment fails or causes issues.

🔁 Common Strategies:

    Blue/Green Deployment:
    
    Traffic can be switched back to the previous (blue) version
    
    Canary Deployment:
    
    Roll out gradually; halt or revert if errors increase
    
    Versioned Artifacts:
    
    Store every release; rollback by redeploying the last working version
    
    Git Revert + Redeploy:
    
    Revert the Git commit and trigger a new build/release
    
    Helm/Kubernetes Rollbacks:
    
    helm rollback <release> or kubectl rollout undo deployment

Best Practice:

Automate rollback detection using monitoring + health checks + alerts
