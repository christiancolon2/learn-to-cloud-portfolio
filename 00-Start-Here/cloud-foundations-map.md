## Phase 0 — Cloud Foundations Map (Mental Model)

### 1) The Big Picture

Cloud = renting **compute, storage, and networking** from a provider (Azure) so you can run things online without owning servers.

**Example: host a small website (what you rent)**

- **Compute:** a VM (virtual Linux computer) to run the web server
- **Storage:** a disk to store the OS + website files
- **Networking:** a public IP + rules to allow web traffic (ports 80/443)

**Goal:** use tools/APIs (Portal/CLI/IaC) to create, change, and delete that setup reliably

- Example: resize the VM bigger, or delete the resource group to remove everything

---

### 2) The Stack (from bottom to top)

**Physical Datacenter**

- Real servers, disks, cables, routers

**Virtualization**

- Hypervisors split big servers into many Virtual Machines (VMs)

**Operating System**

- Linux/Windows run on VMs
- Linux skills = using the OS to run apps, manage files, permissions, services

**Networking**

- IP addresses, DNS, routing, firewalls
- Cloud networking = virtual networks (VNets), subnets, security rules

**Applications**

- Your code + dependencies + runtime
- Runs on VMs, containers, or managed services

**Automation / DevOps Layer**

- Repeatable infrastructure + deployments
- Tools: CLI, scripts, IaC (Terraform/Bicep), CI/CD

---

### 3) The “Cloud Control Plane” vs “Your Workload”

**Control Plane (provider-managed)**

- Azure APIs, Portal, RBAC, subscriptions, billing
- You request resources here

**Data Plane (your workload)**

- Your VMs, containers, storage accounts, databases
- Your app runs here

---

### 4) Azure Core Concepts (beginner map)

**Tenant (Entra ID)**
→ identity directory for org/users

**Subscription**
→ billing + permission boundary

**Resource Group**
→ logical folder for related resources

**Resource**
→ actual thing you create (VM, VNet, Storage, etc.)

Relationship:
Tenant → Subscription → Resource Group → Resources

---

### 5) How You Interact With Cloud

**Portal**

- Click ops (good for learning)

**CLI (Azure CLI)**

- Commands (good for speed + repeatability)

**Infrastructure as Code (IaC)**

- Terraform / Bicep (best for real DevOps workflows)

**CI/CD**

- GitHub Actions / Azure DevOps pipelines run automation

---

### 6) Where Your Week 1 “Hello Azure” fits

You are proving:

- you can authenticate (az login)
- you can query your account (az account show)
- you can create/list/delete resources via CLI
  This proves control-plane access + basic workflow.

---

### 7) What to learn first (priority order)

1. Linux basics (files, permissions, processes, services)
2. Networking basics (IP, DNS, ports, routing)
3. Azure basics (subscription → RG → resource)
4. Automation basics (CLI → scripts → IaC)
