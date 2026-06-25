This is a good follow-up to your CI/CD, Docker, Linux, and Kubernetes content because Terraform is a core interview topic.

### 📱 Caption

🚀 **5 Terraform Questions Asked in Real DevOps Interviews**

Can you answer these?

1️⃣ What is Terraform State?

2️⃣ What's the difference between `terraform plan` and `terraform apply`?

3️⃣ Why do we use a Remote Backend?

4️⃣ Why is DynamoDB used with an S3 Backend?

5️⃣ What's the difference between `count` and `for_each`?

These are some of the most frequently asked Terraform interview questions for DevOps, Cloud, and Platform Engineering roles.

I've created a free repository that includes:

✅ 50+ Terraform Interview Questions
✅ Terraform Cheat Sheet
✅ State Management Explained
✅ Remote Backend (S3 + DynamoDB)
✅ Real Interview Scenarios & Best Practices

💬 Comment **"TERRAFORM"** and I'll share the repository.

📌 Save this reel before your next interview.

Follow **@devops._raj** for daily DevOps interview questions, projects, roadmaps, and career tips. 🚀

#terraform #devops #aws #azure #iac #kubernetes #docker #jenkins #cloud #cloudcomputing #devopsengineer #interviewquestions #techjobs

---

## 📄 `terraform-interview-questions.md`

# 🚀 Terraform Interview Questions & Cheat Sheet

A practical collection of Terraform interview questions, concepts, and commands for DevOps Engineers.

⭐ Star this repository if it helped you.

---

# 📚 Table of Contents

* Terraform Basics
* State Management
* Remote Backend
* Terraform Commands
* Interview Questions
* Scenario-Based Questions
* Best Practices

---

# 🌍 Terraform Basics

## What is Terraform?

Terraform is an Infrastructure as Code (IaC) tool used to provision and manage cloud infrastructure using configuration files.

---

## What is Infrastructure as Code (IaC)?

Infrastructure is defined in code instead of manually creating cloud resources.

Benefits:

* Automation
* Version Control
* Consistency
* Reusability

---

# 📦 Terraform State

## What is Terraform State?

Terraform State (`terraform.tfstate`) stores the mapping between your Terraform configuration and real infrastructure.

Without the state file, Terraform cannot determine what already exists.

---

## Why is Terraform State Important?

* Tracks infrastructure
* Detects changes
* Creates execution plans
* Supports updates without recreating resources

---

# ☁️ Remote Backend

## Why Store State Remotely?

For team collaboration and shared infrastructure.

Example:

* AWS S3
* Azure Storage Account
* Terraform Cloud

---

## Why Use DynamoDB with S3?

DynamoDB provides **state locking**.

It prevents multiple engineers from running `terraform apply` simultaneously and corrupting the state file.

---

# 🚀 Most Used Terraform Commands

Initialize Terraform

```bash
terraform init
```

Preview changes

```bash
terraform plan
```

Create infrastructure

```bash
terraform apply
```

Destroy infrastructure

```bash
terraform destroy
```

Show current state

```bash
terraform show
```

List resources

```bash
terraform state list
```

Format configuration

```bash
terraform fmt
```

Validate configuration

```bash
terraform validate
```

---

# 🎯 Top Interview Questions

## 1. What is Terraform State?

Stores the mapping between Terraform configuration and deployed infrastructure.

---

## 2. Difference Between `terraform plan` and `terraform apply`?

**terraform plan**

* Shows what changes Terraform will make.
* Makes no infrastructure changes.

**terraform apply**

* Executes the plan.
* Creates, updates, or deletes resources.

---

## 3. Why Use Remote State?

* Team collaboration
* Centralized state
* Prevents local state loss
* Enables state locking

---

## 4. Why Use DynamoDB?

To lock the state file and prevent concurrent updates.

---

## 5. Difference Between `count` and `for_each`?

**count**

* Index-based
* Best for identical resources

**for_each**

* Key-based
* Best when each resource has a unique identifier

---

## 6. What Happens During `terraform apply`?

1. Reads configuration
2. Reads state file
3. Compares desired vs current infrastructure
4. Creates an execution plan
5. Applies changes
6. Updates the state file

---

## 7. What is Drift?

When real infrastructure changes outside Terraform, causing the state and actual infrastructure to differ.

---

## 8. What is a Terraform Module?

A reusable collection of Terraform resources.

---

## 9. What is a Provider?

A plugin that allows Terraform to interact with cloud platforms such as AWS, Azure, and GCP.

---

## 10. What is a Resource?

A cloud component managed by Terraform, such as:

* EC2
* S3 Bucket
* Azure Resource Group
* Kubernetes Cluster

---

# 💼 Scenario-Based Questions

### Scenario 1

Two engineers execute `terraform apply` simultaneously.

**Solution:**

Use a remote backend with state locking (for example, S3 + DynamoDB).

---

### Scenario 2

Someone accidentally deletes the local state file.

**Solution:**

Restore it from the remote backend instead of recreating infrastructure.

---

### Scenario 3

Terraform wants to recreate resources unexpectedly.

**Things to check:**

* State file
* Drift
* Resource configuration
* Lifecycle rules

---

# ⭐ Must Know Commands

```bash
terraform init
terraform plan
terraform apply
terraform destroy
terraform fmt
terraform validate
terraform show
terraform state list
terraform output
terraform workspace list
```

---

⭐ If this repository helped you, please Star it.

📸 Follow **@devops._raj** for daily DevOps interview questions, roadmaps, projects, and career tips.
