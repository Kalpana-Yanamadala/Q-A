❓ **1. What is CI/CD and why is it important?**

CI/CD stands for Continuous Integration and Continuous Delivery/Deployment. It automates the software release process to improve speed, consistency, and reliability.

CI ensures code changes are automatically tested and integrated into the main branch frequently.

CD ensures changes can be delivered (or deployed) to production automatically or with minimal manual effort.

**Why it's important:**

Reduces bugs and integration issues

Increases release frequency

Speeds up feedback cycles

Improves team collaboration and code quality

❓ **2. What are the key differences between Continuous Integration, Continuous Delivery, and Continuous Deployment?**

**Concept	Description**
      Continuous Integration (CI)	Developers frequently merge code into a shared branch, triggering automated builds and tests.
      Continuous Delivery (CD)	Ensures the code is always in a deployable state. Deployment to production is manual.
      Continuous Deployment	Similar to CD, but the code is automatically deployed to production once it passes all checks.

**Summary**:

CI → test code early; CD → deploy-ready at all times; Continuous Deployment → goes live automatically.


❓ **3. What is a build pipeline?**

A build pipeline is a sequence of automated steps that compile source code, run tests, and generate deployable artifacts.

    Typical stages:
    
    Checkout code from source control
    
    Install dependencies
    
    Compile/build the code
    
    Run tests (unit/integration)
    
    Package the application (artifact)
    
    Optionally deploy to staging/production

**❓ 4. What are artifacts in a CI/CD pipeline?**

Artifacts are the packaged output of a build process. They are versioned, stored, and used for deployment in later stages.

    Examples:
    
    .jar, .zip, .war files
    
    Docker images
    
    Helm charts
    
    Compiled binaries

Why important:

    Artifacts allow separation of the build and deploy stages, ensuring consistency across environments.

**❓ 5. What tools have you used for CI/CD?**

Answer (customize based on your experience):

I've worked with tools like:

    **GitHub** Actions and GitLab CI for pipeline automation
    
    **Azure DevOps **Pipelines for enterprise-scale build and release
    
    **Jenkins** for custom CI jobs
    
    **SonarQube** for code quality checks
    
    **Docker** and **Kubernetes** for container-based deployment

❓** 6. What are common challenges in a CI/CD setup?**

Answer:

Flaky Tests: Tests that randomly fail or pass, causing false negatives

    **Long Build Times**: Affects developer productivity
    
   ** Secrets Management**: Storing and using credentials securely
    
    **Environment Drift**: Inconsistent environments across stages
    
    **Rollback Complexity**: Handling failed deployments safely
    
    **Dependency Conflicts**: Breaks due to external library updates
