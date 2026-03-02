# Roadmap (6–8 Weeks) — Learn to Cloud Bootcamp (Azure)

## Purpose

Complete the Learn to Cloud Bootcamp in 6–8 weeks with strong proof-of-work artifacts for each phase, using **Azure** as the cloud platform focus.

## Rules (Non-Negotiable)

- **One cloud only:** Azure
- **Ship weekly:** at least **1 proof artifact** + **1 short write-up**
- **Document as you go:** every repo must have a clean README with steps + screenshots
- **Finish > perfect:** complete the full roadmap before polishing

---

## Weekly Cadence (Repeat Every Week)

### Minimum Weekly Outputs

- **1 Proof Artifact** (diagram, lab walkthrough, script, repo milestone, or deployment)
- **1 Weekly Log** (what you learned, what you shipped, what’s next)
- **Clean Notes** (not raw dumps—organized and readable)

### Suggested Weekly Rhythm

- **Mon–Fri:** lessons + labs + notes
- **Sat:** capstone/proof day (ship something real)
- **Sun:** review + weekly log + cleanup + plan next week

---

## Milestone Checklist (What “Done” Looks Like)

By the end of this roadmap, you will have:

- Phase-by-phase notes and labs in a consistent structure
- A complete **Learning Journal API** project (FastAPI + DB)
- An **Azure Deployment Capstone** (compute + networking + identity + monitoring + cost controls)
- A **DevOps Foundations** repo (Docker + CI/CD + Terraform baseline)
- A **Security Hardening** deliverable (secrets + IAM + network controls + monitoring + incident notes)

---

# Week-by-Week Plan

## Week 1 — Phase 0 Foundations + Start Phase 1 Setup

### Goals

- Build correct mental models for Linux, networking, programming, cloud, and DevOps
- Finish environment setup and verify Azure CLI workflow

### Deliverables

- `phase-0-cloud-foundations-map.md` (1 page)
- `phase-0-glossary.md` (25–40 terms with simple examples)
- `week-01-hello-azure.md` (Azure CLI proof)

### Azure “Hello World” (Proof)

Document commands + screenshots:

- `az login`
- `az account show`
- Create resource group (CLI)
- List it (CLI)
- Delete it (CLI)

### Done When

- Foundations map + glossary committed
- Azure CLI workflow documented and repeatable

---

## Week 2 — Phase 1 Linux & Bash (Deep)

### Goals

- Get comfortable in the terminal
- Build repeatable workflows: CLI, SSH, Git, and basic automation

### Deliverables

- CLI cheat sheet (top 30 commands)
- `system_report.sh` (or another useful bash automation script)
- Linux CTF walkthrough (clear steps + screenshots)

### Done When

- You can repeat the labs without looking up every command
- Script runs cleanly and README explains how to use it
- CTF walkthrough is readable and complete

---

## Week 3 — Phase 2 Networking Fundamentals

### Goals

- Understand IP/subnetting, routing, DNS, HTTP, ports/protocols
- Be able to explain how traffic flows end-to-end

### Deliverables

- Networking concept map (IP → subnet → routing → DNS → HTTP)
- Ports & protocols cheat sheet (with real examples + test commands)
- Network Troubleshooting Lab walkthrough + screenshots

### Done When

- You can explain the difference between DNS vs routing vs firewall vs app problems
- You have a clean lab write-up that someone else can follow

---

## Week 4 — Phase 3 Programming Fundamentals (Python + FastAPI + DB)

### Goals

- Build the Learning Journal API project with clean structure and documentation
- Understand request/response flow and database integration

### Deliverables

- `learning-journal-api/` with:
  - Working FastAPI app
  - Database integration
  - Clean README: setup, run, endpoints, examples
- `docs/architecture-notes.md` (1–2 pages)
- One extra feature (choose one):
  - search
  - pagination
  - improved validation
  - improved error handling
  - basic auth (simple token)

### Done When

- Project runs from scratch using your README
- You can explain the architecture and data flow

---

## Week 5 — Phase 4 Azure Cloud Platform Fundamentals (Deployment)

### Goals

- Deploy the app on Azure with real cloud components
- Add monitoring and cost controls

### Deliverables

- Azure Deployment Capstone repo with:
  - Architecture diagram
  - Step-by-step deployment guide
  - Verification checklist (how to confirm it works)
  - Screenshots of Azure resources
- Cost controls proof (budget/alerts) documented

### Required Components (High Level)

- Resource Group
- Compute (App Service or VM)
- Identity/Access (basic RBAC / Entra concepts)
- Cloud networking (as required by your deployment path)
- Database service (managed where possible)
- Monitoring (Azure Monitor / logs)

### Done When

- A reviewer can follow your steps and reproduce the deployment
- You can point to monitoring/logs and cost controls

---

## Week 6 — Phase 5 DevOps Fundamentals (Docker + CI/CD + Terraform Baseline)

### Goals

- Containerize the app
- Build basic automation for build/test
- Provision baseline Azure infra with Terraform (keep it small and real)

### Deliverables

- Dockerized Journal API (Dockerfile + run instructions)
- CI pipeline (GitHub Actions is fine):
  - lint/test and/or build on push
- Terraform baseline for Azure:
  - minimum: resource group + one additional resource
  - include `plan/apply/destroy` steps

### Done When

- You can build and run your container locally
- CI runs automatically on push
- Terraform workflow is documented and repeatable

---

## Week 7 — Phase 6 Securing Your Cloud Apps (Azure Security Baseline)

### Goals

- Implement basic security hardening and document it clearly
- Demonstrate secrets handling, least privilege, and monitoring awareness

### Deliverables

- Security checklist + implementation proof
- Secrets approach documented (preferred: Azure Key Vault or secure app settings)
- RBAC notes (who can do what)
- Network controls summary (only expose what’s needed)
- Monitoring + incident notes (what to do first if something breaks)

### Done When

- No secrets in code or repo
- Permissions are deliberate and documented
- You can show logs/monitoring and describe first-response steps

---

## Week 8 (Optional Buffer) — Polish + Packaging

### Goals

- Make the portfolio easy to evaluate in 5 minutes
- Clean repos, screenshots, and navigation

### Deliverables

- Hub README “Start Here” upgrade:
  - quick overview
  - links to best artifacts
  - screenshots
- Tighten READMEs across repos
- Add final “What I built / What I learned” summary

### Done When

- Someone can land on the hub repo and immediately understand your skill progression
- Everything is linked, readable, and reproducible

---

# Proof-of-Work Index (What to Link in the Hub README)

- Phase 0: Foundations map + glossary
- Phase 1: Linux CTF walkthrough + bash script
- Phase 2: Networking troubleshooting lab + concept map
- Phase 3: Learning Journal API + architecture notes
- Phase 4: Azure deployment capstone + diagram + verification checklist
- Phase 5: Docker + CI pipeline + Terraform baseline
- Phase 6: Security checklist + secrets/IAM/network controls + monitoring notes

---

# Weekly Log Template (Copy/Paste)

## Week \_\_

**Goal:**  
**What I completed:**

- **What I shipped (links):**

- **Biggest lessons:**

- **Problems / blockers:**

- **Next week plan:**

-
