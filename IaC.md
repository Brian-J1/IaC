# Infrastructure as code (IaC)

## What is Infrastructure as Code (IaC)?

**Infrastructure as Code (IaC)** is the practice of managing and provisioning computing infrastructure (like servers, networks, databases) using machine-readable **code** instead of manual processes. It allows automation, consistency, and version control of infrastructure.

---
#  Benefits of Infrastructure as Code (IaC)
##  **Consistency & Repeatability**
- Eliminates human error by automating infrastructure provisioning.
- Ensures environments are identical across dev, test, and production.

##  **Speed & Efficiency**
- Automates resource creation in minutes.
- Reduces setup time for new environments and deployments.

## What is Configuration Management?

**Configuration Management** is the process of **maintaining and managing software and system configurations** on servers and other resources. It ensures consistency across environments by automating tasks like package installation, updates, and settings.

---

## What is Orchestration?

**Orchestration** is the automated coordination and management of complex IT workflows and services — like deploying multi-tier applications, scaling infrastructure, or connecting containers. It handles the **big picture** beyond single-node configuration.

---

## What is Ansible?

**Ansible** is an open-source **automation tool** for configuration management, application deployment, and orchestration. It uses simple **YAML files (Playbooks)** and communicates with **target nodes over SSH**, requiring **no agents** on the managed machines.

---

## How Does Ansible Work?

1. You write tasks in YAML (Playbooks).
2. You define target nodes in an Inventory file.
3. Ansible runs commands from a **Control Node** via **SSH**.
4. The target nodes execute tasks without needing a client or agent.

---

### Ansible Architecture Diagram

![Ansible Diagram](https://www.devopsschool.com/blog/wp-content/uploads/2019/07/Understanding-Ansible-Architecture-using-diagram1.png)

> *Control Node = Where you run Ansible*  
> *Managed Nodes = Your target servers*
