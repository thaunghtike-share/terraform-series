# ![Terraform](https://raw.githubusercontent.com/hashicorp/terraform-website/master/content/source/assets/images/logo-hashicorp-3f10732f.svg) Advanced Terraform & Platform Engineering Bootcamp

## 12 Weeks — Real Enterprise Hands-on Training

---

# Course Overview

This course is designed for students who already understand basic Terraform concepts and want to move into real-world enterprise infrastructure engineering.

This is NOT a beginner Terraform course.

Students will learn how real Platform Engineers build and manage:

* Enterprise Terraform Architecture
* Remote State Infrastructure
* Reusable Terraform Modules
* GitHub Actions CI/CD
* Azure OIDC Authentication
* Terraform Cloud Workflows
* terraform-docs Automation
* Terragrunt Architecture
* Atmos Platform Orchestration
* Golden Path Infrastructure
* Internal Developer Platform Concepts

---

# Technologies Used

* Terraform
* Azure
* GitHub Actions
* Azure OIDC
* Terraform Cloud
* terraform-docs
* Terragrunt
* Atmos

---

# Real Infrastructure Architecture Used Throughout Course

```text
terraform-platform/
├── 00_resource_groups
├── 01_networking
├── 02_identity
├── 03_storage
├── 04_compute
├── 05_databases
├── 06_monitoring
├── modules/
├── environments/
│   ├── dev
│   ├── uat
│   └── prod
├── .github/workflows
├── docs/
├── terragrunt/
└── atmos/
```

---

# Week 1 — Terraform Foundations

## Goal

Understand real Terraform workflow and enterprise project structure.

---

## Day 1 — Terraform Fundamentals

### Topics

* Infrastructure as Code
* Terraform Workflow
* Providers
* Resources
* Variables
* Outputs
* Terraform State

### Hands-on

* Create Azure Resource Group
* Create Storage Account
* Create Virtual Network
* Use Variables and Outputs

### Real Lab

```text
Deploy complete development environment foundation
```

---

## Day 2 — Terraform Language Deep Dive

### Topics

* String
* Number
* Bool
* List
* Map
* Object
* Functions
* Conditional Logic
* for_each
* count

### Hands-on

* Create multiple VNets dynamically
* Dynamic subnet creation
* Environment-based resource sizing

### Real Lab

```text
Single codebase for dev, uat and prod environments
```

---

## Day 3 — Terraform Project Structure

### Topics

* providers.tf
* variables.tf
* outputs.tf
* locals.tf
* versions.tf
* terraform.tfvars

### Hands-on

* Refactor messy code into enterprise structure

### Real Lab

```text
Convert beginner Terraform project into enterprise layout
```

---

# Week 2 — Terraform State & Backend Engineering

## Goal

Learn enterprise state management.

---

## Day 1 — Terraform State Deep Dive

### Topics

* tfstate internals
* Drift detection
* State locking
* Sensitive data risks

### Hands-on

* Inspect tfstate
* Import existing resource
* Simulate infrastructure drift

### Real Lab

```text
Recover broken infrastructure from state mismatch
```

---

## Day 2 — Azure Remote State Backend

### Topics

* Azure Blob backend
* Backend configuration
* State locking
* Environment isolation

### Hands-on

* Configure remote backend
* Separate backend per layer

### Real Lab

```text
Move local infrastructure to enterprise remote state
```

---

## Day 3 — Multi Layer Infrastructure

### Topics

* Layered architecture
* Dependency management
* terraform_remote_state

### Hands-on

* Connect networking layer with compute layer
* Connect storage layer with database layer

### Real Lab

```text
Build complete layered infrastructure platform
```

---

# Week 3 — Terraform Modules

## Goal

Build reusable infrastructure platforms.

---

## Day 1 — Module Fundamentals

### Topics

* Root module
* Child module
* Inputs
* Outputs
* Module structure

### Hands-on

* Build reusable Resource Group module
* Build reusable Storage module

### Real Lab

```text
Create reusable infrastructure library
```

---

## Day 2 — Advanced Module Design

### Topics

* Dynamic modules
* Environment-based modules
* Naming standards

### Hands-on

* Reusable VNet module
* Reusable VM module

### Real Lab

```text
One module supporting multiple environments
```

---

## Day 3 — Enterprise Module Workflow

### Topics

* Module versioning
* Shared platform modules
* Private module strategy

### Hands-on

* Shared organization module repository

### Real Lab

```text
Platform engineering style module architecture
```

---

# Week 4 — Enterprise Infrastructure Design

## Goal

Think like a Platform Engineer.

---

## Day 1 — Environment Architecture

### Topics

* Dev/UAT/Prod strategy
* Naming standards
* Folder strategy

### Hands-on

* Build multi-environment platform

### Real Lab

```text
Enterprise environment separation
```

---

## Day 2 — Infrastructure Standards

### Topics

* Tagging strategy
* Naming conventions
* Shared variables
* Shared locals

### Hands-on

* Standardize all infrastructure resources

### Real Lab

```text
Enforce organization standards
```

---

## Day 3 — Platform Repository Design

### Topics

* Monorepo
* Multi repo
* Layered repositories

### Hands-on

* Build enterprise repository structure

### Real Lab

```text
Production-ready Terraform platform repository
```

---

# Week 5 — GitHub Actions for Terraform

## Goal

Automate infrastructure delivery.

---

## Day 1 — Terraform CI Pipeline

### Topics

* GitHub Actions
* terraform fmt
* validate
* plan

### Hands-on

* CI validation workflow

### Real Lab

```text
Automatic Terraform validation pipeline
```

---

## Day 2 — Terraform Apply Pipeline

### Topics

* workflow_dispatch
* Environment approvals
* Production safety

### Hands-on

* Multi-environment apply workflow

### Real Lab

```text
Production infrastructure deployment pipeline
```

---

## Day 3 — Secure Pipeline Design

### Topics

* Secrets management
* tfvars generation
* Secure workflows

### Hands-on

* Generate secure tfvars dynamically

### Real Lab

```text
Secretless deployment workflow
```

---

# Week 6 — OIDC & Modern IAM

## Goal

Eliminate static secrets.

---

## Day 1 — OIDC Fundamentals

### Topics

* Modern identity management
* Workload identity
* Federated credentials

### Hands-on

* Azure App Registration
* Federated credential setup

### Real Lab

```text
GitHub Actions login without secrets
```

---

## Day 2 — GitHub Actions + Azure OIDC

### Hands-on

* Configure azure/login
* Configure Terraform OIDC authentication

### Real Lab

```text
Enterprise-grade Terraform authentication
```

---

## Day 3 — RBAC & Permission Design

### Topics

* Least privilege
* Storage Blob Data Contributor
* Reader role
* Scope strategy

### Hands-on

* Secure Terraform backend access

### Real Lab

```text
Enterprise RBAC implementation
```

---

# Week 7 — Terraform Security & Validation

## Goal

Build secure infrastructure pipelines.

---

## Day 1 — Terraform Security Tools

### Topics

* tfsec
* checkov
* tflint

### Hands-on

* Security scanning pipeline

### Real Lab

```text
Detect insecure infrastructure automatically
```

---

## Day 2 — Infrastructure Compliance

### Topics

* Prevent public exposure
* Security standards
* Policy validation

### Hands-on

* Secure storage accounts
* Secure networking rules

### Real Lab

```text
Enterprise security enforcement
```

---

## Day 3 — Troubleshooting Terraform

### Hands-on

* State recovery
* Lock issues
* Broken dependencies

### Real Lab

```text
Recover failed production deployment
```

---

# Week 8 — Terraform Cloud Enterprise Workflow

## Goal

Learn enterprise Terraform operations.

---

## Day 1 — Terraform Cloud Fundamentals

### Hands-on

* Create workspace
* Connect GitHub repository

### Real Lab

```text
Remote execution workflow
```

---

## Day 2 — Team Collaboration

### Topics

* Workspace design
* Variable sets
* RBAC

### Hands-on

* Multi-team infrastructure workflow

### Real Lab

```text
Shared infrastructure operations
```

---

## Day 3 — Terraform Cloud CI/CD

### Hands-on

* VCS integration
* Remote plans
* Apply approvals

### Real Lab

```text
Enterprise infrastructure automation
```

---

# Week 9 — terraform-docs & Developer Experience

## Goal

Improve platform usability.

---

## Day 1 — terraform-docs

### Hands-on

* Generate README automatically
* Inject vs replace

### Real Lab

```text
Enterprise Terraform documentation
```

---

## Day 2 — CI/CD Documentation Automation

### Hands-on

* terraform-docs GitHub Actions workflow

### Real Lab

```text
Auto-update infrastructure documentation
```

---

## Day 3 — Developer Friendly Infrastructure

### Topics

* Platform usability
* Infrastructure templates
* Self-service concepts

### Real Lab

```text
Golden path Terraform template
```

---

# Week 10 — Terragrunt at Scale

## Goal

Manage large infrastructure efficiently.

---

## Day 1 — Terragrunt Fundamentals

### Hands-on

* Convert Terraform repo to Terragrunt

### Real Lab

```text
Reduce duplicated infrastructure code
```

---

## Day 2 — Environment Management

### Hands-on

* Shared configurations
* Environment inheritance

### Real Lab

```text
Centralized platform configuration
```

---

## Day 3 — Terragrunt CI/CD

### Hands-on

* Multi-environment Terragrunt deployment

### Real Lab

```text
Enterprise Terragrunt automation
```

---

# Week 11 — Atmos & Platform Engineering

## Goal

Modern platform orchestration.

---

## Day 1 — Atmos Fundamentals

### Hands-on

* Atmos stack configuration

### Real Lab

```text
Centralized infrastructure orchestration
```

---

## Day 2 — Platform Composition

### Hands-on

* Shared platform components
* Tenant environments

### Real Lab

```text
Platform engineering infrastructure model
```

---

## Day 3 — Golden Path Infrastructure

### Topics

* Internal Developer Platform
* Golden path concept
* Self-service infrastructure

### Hands-on

* Standardized environment templates

### Real Lab

```text
Developer self-service infrastructure platform
```

---

# Week 12 — Final Enterprise Platform Project

## Final Project

Students build complete enterprise infrastructure platform:

```text
✅ Multi-layer Terraform architecture
✅ Remote state backend
✅ Reusable modules
✅ GitHub Actions CI/CD
✅ Azure OIDC authentication
✅ Terraform Cloud workflow
✅ terraform-docs automation
✅ Terragrunt structure
✅ Atmos orchestration
✅ Golden path infrastructure
✅ Enterprise repository structure
```

---

# Final Outcome

After completing this program, students will understand:

* Enterprise Terraform Workflow
* Platform Engineering Concepts
* Infrastructure Automation
* Secure CI/CD Pipelines
* OIDC Authentication
* Infrastructure at Scale
* Golden Path Engineering
* Internal Developer Platform Design

---

# Recommended Student Requirements

* Basic Linux Knowledge
* Basic Git Knowledge
* Basic Terraform Knowledge
* Azure Account
* GitHub Account

---

# Teaching Style

✅ Real World Labs
✅ Production Style Infrastructure
✅ Enterprise Repository Structure
✅ CI/CD Automation
✅ Troubleshooting Sessions
✅ Platform Engineering Mindset
✅ Real Production Workflow
✅ Infrastructure Design Thinking
