# 🏗️ Terraform Cheat Sheet

A quick reference guide for Terraform commands every DevOps Engineer should know.

⭐ Star this repository if it helps you.

---

# 🚀 Getting Started

## Initialize Terraform

```bash
terraform init
```

Downloads providers and initializes the working directory.

---

## Check Terraform Version

```bash
terraform version
```

---

# 📝 Planning & Deployment

## Preview Changes

```bash
terraform plan
```

Shows what Terraform will create, modify, or destroy.

---

## Apply Changes

```bash
terraform apply
```

Creates or updates infrastructure.

---

## Auto Approve

```bash
terraform apply -auto-approve
```

Skips confirmation prompt.

---

## Destroy Infrastructure

```bash
terraform destroy
```

Deletes all managed resources.

---

# ✅ Validation & Formatting

## Validate Configuration

```bash
terraform validate
```

Checks for syntax and configuration errors.

---

## Format Code

```bash
terraform fmt
```

Formats Terraform files using standard style.

---

# 📦 State Management

## View Current State

```bash
terraform show
```

Displays current infrastructure state.

---

## List Managed Resources

```bash
terraform state list
```

---

## Show Resource Details

```bash
terraform state show <resource-name>
```

Example:

```bash
terraform state show azurerm_resource_group.rg
```

---

# 📤 Outputs

## View Outputs

```bash
terraform output
```

---

## View Specific Output

```bash
terraform output public_ip
```

---

# 🌍 Workspaces

## List Workspaces

```bash
terraform workspace list
```

---

## Create Workspace

```bash
terraform workspace new dev
```

---

## Switch Workspace

```bash
terraform workspace select prod
```

---

# 📂 Modules

Example:

```hcl
module "vpc" {
  source = "./modules/vpc"

  cidr = "10.0.0.0/16"
}
```

Modules help reuse infrastructure code.

---

# 🔒 Remote State

Example Backend:

```hcl
terraform {
  backend "s3" {
    bucket         = "terraform-state"
    key            = "prod/terraform.tfstate"
    region         = "ap-south-1"
    dynamodb_table = "terraform-lock"
  }
}
```

Benefits:

* Shared State
* State Locking
* Team Collaboration
* Backup

---

# 📚 Most Used Terraform Commands

```bash
terraform init
terraform plan
terraform apply
terraform destroy
terraform validate
terraform fmt
terraform show
terraform output
terraform state list
terraform workspace list
terraform workspace new dev
terraform workspace select dev
```

---

# 🎯 Terraform Interview Tips

✅ Understand Terraform State

✅ Know the difference between `plan` and `apply`

✅ Learn Remote Backend concepts

✅ Know why DynamoDB is used with S3

✅ Understand Modules

✅ Learn Variables & Outputs

✅ Practice Workspaces

---

# 🚀 Common Interview Questions

### What is Terraform State?

Tracks infrastructure managed by Terraform.

---

### Difference between `terraform plan` and `terraform apply`?

* `plan` → Preview changes
* `apply` → Execute changes

---

### Why use Remote State?

To enable team collaboration and centralized state management.

---

### Why use DynamoDB with S3?

To provide state locking and prevent concurrent `terraform apply` operations.

---

### What are Modules?

Reusable Terraform configurations that reduce duplication.

---

### What are Workspaces?

Workspaces allow you to manage multiple environments (Dev, QA, Prod) using the same configuration.

---

⭐ Star this repository if it helped you.

📸 Follow **@devops._raj** for daily DevOps interview questions, cheat sheets, projects, and career tips.
