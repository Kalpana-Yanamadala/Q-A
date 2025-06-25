❓ **1. What is Jenkins/GitHub Actions/Azure DevOps/GitLab CI/CD?**

These are popular CI/CD automation tools used to build, test, and deploy applications:

**Tool	Description**

    Jenkins	Open-source automation server. Highly customizable with plugins. Widely used in enterprises.
    GitHub Actions	CI/CD built into GitHub. Uses YAML files to define workflows. Great for GitHub-native projects.
    Azure DevOps	Microsoft’s end-to-end DevOps platform offering build/release pipelines, boards, repos, and artifacts.
    GitLab CI/CD	Integrated with GitLab. Offers pipeline automation, container registry, and security features in one platform.

👉 These tools help automate the software lifecycle: code integration, testing, packaging, and deployment.

❓ **2. What is version control and why is it important for CI/CD?**

Version control (e.g., Git) is a system that tracks changes to source code over time.

Why it's important in CI/CD:

    Tracks code history and collaboration
    
    Triggers CI/CD pipelines automatically on code changes (e.g., push, pull request)
    
    Enables branching strategies (e.g., feature branches, mainline development)
    
    Helps roll back or troubleshoot issues in deployments

🔑 CI/CD relies heavily on version control to detect changes, merge code safely, and automate testing.

❓** 3. What is the purpose of a build server?**

A build server is a machine (or agent) that executes automated build and test jobs triggered by CI/CD pipelines.

Functions:

    Clones code from source control
    
    Installs dependencies
    
    Compiles/builds the application
    
    Runs unit and integration tests
    
    Packages and stores artifacts

Examples: Jenkins Agent, GitHub-hosted runner, Azure DevOps agent, GitLab runner.

❓ **4. What is the difference between build and release pipelines?**

Pipeline Type	Description

    Build Pipeline	Focuses on compiling code, running tests, creating artifacts (e.g., .jar, Docker images). Often triggered on code commits.
    Release Pipeline	Focuses on deploying those artifacts to environments (Dev, QA, Prod), sometimes with approvals or gating. Can include configuration, rollback logic, etc.

Summary:

    Build = "create and test"
    
    Release = "deploy and promote"

❓ **5. What are triggers in a pipeline?**

Triggers determine when a pipeline starts automatically.

Types of triggers:

    Push trigger: Starts pipeline when code is pushed to a branch
    
    Pull Request (PR) trigger: Starts pipeline on PR creation/update
    
    Scheduled trigger: Runs pipeline on a set schedule (e.g., daily at midnight)
    
    Manual trigger: Manually initiated by a developer/operator
    
    Pipeline trigger: Triggered by another pipeline (chained builds)

Purpose:

Ensures timely and automated validation and deployment of code.
