# ⚙️ CI/CD Interview Questions
### If you know these, you're already ahead of 80% of freshers.

> 📸 Follow [@devops._raj](https://www.instagram.com/devops._raj) — Daily DevOps tips & interview prep  
> 💬 Comment **"CICD"** on the reel → get this repo link in your DM 🚀

---

## 🔥 Top 10 CI/CD Interview Questions

---

### 1. What is CI/CD?

**CI (Continuous Integration)** — developers push code frequently. Every push automatically builds and tests the code.

**CD (Continuous Delivery)** — code is always ready to deploy. A human approves the final push to production.

**CD (Continuous Deployment)** — goes one step further. Every passing build is automatically deployed to production. No human needed.

> Simple way to remember: CI = merge safely. CD = ship safely.

---

### 2. What are the stages of a CI/CD pipeline?

```
Code Push → Build → Test → Artifact → Deploy to Staging → Deploy to Production
```

| Stage | What happens |
|-------|-------------|
| Code Push | Developer pushes to GitHub/GitLab |
| Build | Code is compiled, dependencies installed |
| Test | Unit tests, integration tests run automatically |
| Artifact | A deployable package is created (Docker image, JAR) |
| Staging | Deploy to a test environment for QA |
| Production | Deploy to live environment |

---

### 3. What is the difference between Continuous Delivery and Continuous Deployment?

| | Continuous Delivery | Continuous Deployment |
|-|--------------------|-----------------------|
| Deploy to staging | ✅ Automatic | ✅ Automatic |
| Deploy to production | ❌ Manual approval needed | ✅ Fully automatic |
| Best for | Apps needing human sign-off | High-confidence, fast teams |

---

### 4. What tools are used for CI/CD?

| Tool | Best for |
|------|----------|
| **GitHub Actions** | GitHub repos, easiest to start |
| **GitLab CI** | Full DevOps platform, self-hosted |
| **Jenkins** | Most used in enterprise |
| **CircleCI** | Fast setup, good free tier |
| **ArgoCD** | GitOps-based CD for Kubernetes |

> In 2026 — **GitHub Actions** is the most in-demand. Learn this first.

---

### 5. What is a pipeline-as-code?

Instead of configuring your pipeline through a UI, you write it as a YAML file and store it in your repo.

**Why it matters:**
- Pipeline is version-controlled
- Anyone on the team can review and change it
- Easy to replicate across projects

Example — GitHub Actions:
```yaml
name: CI Pipeline
on: [push]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - run: echo "Build and test here"
```

---

### 6. What is a build artifact?

An artifact is the output of your build stage — something deployable.

Examples:
- A Docker image
- A `.jar` or `.war` file (Java)
- A `.zip` of compiled frontend code

Artifacts are stored in registries like Docker Hub, AWS ECR, or GitHub Packages, then pulled during deployment.

---

### 7. How do you store secrets in a CI/CD pipeline?

**Never hardcode secrets in your pipeline file.** Use:

- **GitHub Actions** → GitHub Secrets (`${{ secrets.MY_SECRET }}`)
- **Jenkins** → Jenkins Credentials Store
- **GitLab CI** → CI/CD Variables
- **Production** → HashiCorp Vault or AWS Secrets Manager

Rule of thumb: if it's sensitive, it should never appear in your repo — not even in `.env` files.

---

### 8. What is a rollback? How do you handle it in CI/CD?

A rollback means reverting to the last working version when a deployment fails.

**Ways to handle it:**
- **Blue-Green deployment** — keep old version running, switch traffic back instantly
- **Canary deployment** — only a % of users see the new version, roll back before full rollout
- **Kubernetes** — `kubectl rollout undo deployment/app-name`
- **Feature flags** — turn off a broken feature without redeploying

---

### 9. What is the difference between blue-green and canary deployment?

| | Blue-Green | Canary |
|-|-----------|--------|
| How it works | Two environments — switch traffic all at once | Gradually shift % of traffic to new version |
| Rollback speed | Instant | Fast |
| Risk | Low | Very low |
| Cost | Higher (2x infra) | Normal |
| Best for | Simple apps | High-traffic, risk-sensitive apps |

---

### 10. How do you test in a CI/CD pipeline?

Three types of tests that should run automatically:

**Unit tests** — test individual functions. Fast. Run on every commit.

**Integration tests** — test how services work together. Run after build.

**End-to-end (E2E) tests** — simulate a real user flow. Run before production deploy.

> Fail fast = catch bugs early = cheaper to fix. That's the whole point of CI.

---

## ⚡ Bonus — 3 Questions Asked in Real Interviews

**Q: Your pipeline is passing but production is broken. What do you do?**
> Check if the test coverage is adequate. Tests might be passing but not covering the right cases. Add integration/E2E tests. Also check environment differences between staging and prod.

**Q: How do you speed up a slow pipeline?**
> Cache dependencies, run jobs in parallel, use smaller Docker base images, skip unnecessary stages on non-main branches.

**Q: What is shift-left testing?**
> Moving testing earlier in the pipeline — catching bugs at the code stage instead of after deployment. Saves time and cost.

---


*⭐ Star this repo if it helped you!*

> 📸 **More interview questions daily → [@devops._raj](https://www.instagram.com/devops._raj)**  
> 💬 Comment **"CICD"** on the reel to get this link in your DM 🚀
>
<p align="center">
  <img src="https://komarev.com/ghpvc/?username=PreethamRaj9121&label=Repo%20Views&color=0e75b6&style=flat" />
</p>
