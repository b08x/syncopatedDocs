---
layout: page
title: Backlog
toc: true
permalink: /docs/backlog
---


# Yeah

This backlog organizes the suggestions and areas to explore into epics and user stories to guide development.


## Epics:

1. **Containerization and Portability**
2. **Enhanced Configuration and Security**
3. **Simplified User Onboarding and Use Cases**
4. **Advanced Resource Management and Monitoring**
5. **IDE Integration and Developer Experience**
6. **Robust Testing and Quality Assurance**
7. **Open Source Community Building**

## User Stories:

**Epic 1: Containerization and Portability**

* **As a developer, I want to use Docker to deploy the AI/NLP development environment so that I can ensure consistency and portability across different machines.**
    * Tasks:
        * Containerize core services (Graylog, Langfuse, databases, Redis).
        * Containerize LLM services (Ollama, LocalAI).
        * Containerize AI development platforms (Flowise, Dify.ai, Agenta).
        * Provide Docker Compose files for easy multi-container orchestration.
* **As a developer, I want to have the option to use Podman as an alternative to Docker for containerization.**
    * Tasks:
        * Ensure compatibility with Podman for all containerized components.
        * Provide Podman Compose files alongside Docker Compose files.

**Epic 2: Enhanced Configuration and Security**

* **As a developer, I want to securely manage sensitive configuration data (API keys, database credentials) so that my information is protected.**
    * Tasks:
        * Implement Ansible Vault support for encrypting and managing sensitive variables.
        * Provide clear documentation and examples on how to use Ansible Vault with the collection.
* **As a developer, I want to configure the firewall to allow only necessary traffic to my local development environment.**
    * Tasks:
        * Develop Ansible roles to configure firewall rules for common services and ports.
        * Allow users to customize firewall rules based on their specific needs.

**Epic 3: Simplified User Onboarding and Use Cases**

* **As a new user, I want access to pre-configured Ansible playbooks for common AI/NLP development scenarios so that I can get started quickly.**
    * Tasks:
        * Create template playbooks for:
            * LLM Finetuning Setup
            * AI Chatbot Development
            * Text Generation and Summarization
* **As a developer, I want to easily choose which components to install and configure without having to manually edit complex playbooks.**
    * Tasks:
        * Develop an interactive menu-driven setup process (using Ansible's `prompt` module or similar).

**Epic 4: Advanced Resource Management and Monitoring**

* **As a developer, I want to monitor the resource utilization (CPU, memory, GPU) of my AI/NLP workloads within my local development environment.**
    * Tasks:
        * Integrate resource monitoring tools (e.g., `htop`, `nvidia-smi`) into the Ansible roles.
        * Provide dashboards or reports within the development environment to visualize resource usage.
* **As a developer, I want to be able to easily adjust the resource limits (CPU cores, memory, etc.) allocated to different components of the environment.**
    * Tasks:
        * Implement Ansible variables or configuration files to control resource allocation.

**Epic 5: IDE Integration and Developer Experience**

* **As a developer, I want my IDE (VS Code, PyCharm) to automatically recognize the Ansible-provisioned environment so that I have a seamless development workflow.**
    * Tasks:
        * Research and implement IDE extensions or plugins that can:
            * Detect and configure Python virtual environments created by the Ansible roles.
            * Provide code completion and linting based on the installed libraries.
* **As a developer, I want easy access to documentation and help resources from within my development environment.**
    * Tasks:
        * Provide links to relevant documentation, tutorials, and community forums.

**Epic 6: Robust Testing and Quality Assurance**

* **As a contributor, I want to ensure that my code changes do not break existing functionality.**
    * Tasks:
        * Implement a comprehensive test suite using Molecule for testing Ansible roles.
        * Cover different operating systems and configurations in the tests.
* **As a maintainer, I want to have confidence that new releases of the collection are stable and reliable.**
    * Tasks:
        * Set up a CI/CD pipeline (e.g., using GitHub Actions, GitLab CI) to automate testing and deployment.

**Epic 7: Open Source Community Building**

* **As a potential contributor, I want clear guidelines on how to contribute to the project.**
    * Tasks:
        * Create a detailed CONTRIBUTING.md file outlining the contribution process.
        * Define coding style guidelines and best practices.
* **As a member of the community, I want to be able to engage with other users and developers.**
    * Tasks:
        * Set up communication channels (e.g., Discord server, forum) for discussions and support.
        * Encourage community contributions and feedback.
