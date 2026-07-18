# 🚨 Production Troubleshooting Guide

## Scenario #1

### Problem

Production is DOWN.

CPU: 20%

Memory: Normal

Users can't log in.

---

## Step 1 — Confirm the Issue

Questions:

- Is every user affected?
- Is it only login?
- Is the website loading?
- Any recent deployment?

---

## Step 2 — Check Kubernetes

```bash
kubectl get pods
kubectl get svc
kubectl get ingress
kubectl get events --sort-by=.metadata.creationTimestamp
```

Look for:

- CrashLoopBackOff
- ImagePullBackOff
- Pending Pods
- Failed Events

---

## Step 3 — Application Logs

```bash
kubectl logs <pod-name>

kubectl logs <pod-name> --previous
```

Things to look for:

- Database timeout
- NullPointerException
- Authentication failures
- Secret missing
- Environment variable missing

---

## Step 4 — Recent Deployment

Questions:

- Was a deployment done today?
- Configuration changed?
- Secret rotated?
- Image updated?

Check:

- Jenkins
- GitHub Actions
- GitLab
- ArgoCD

---

## Step 5 — Database

Verify:

- Database is running
- Connection string
- Credentials
- Network connectivity

---

## Step 6 — Authentication

Verify:

- OAuth
- JWT
- LDAP
- Active Directory
- Session Store

---

## Step 7 — Networking

```bash
kubectl get ingress

kubectl get svc

nslookup example.com
```

Check:

- DNS
- Load Balancer
- SSL Certificate
- Network Policy

---

## Common Root Causes

- Bad deployment
- Database down
- Expired Secret
- Wrong ConfigMap
- Ingress issue
- DNS issue
- Authentication failure
- Network Policy
- Expired SSL

---

## Interview Tip

Never answer:

"I'll restart the server."

Instead explain:

1. Gather information
2. Check logs
3. Isolate the issue
4. Identify the root cause
5. Fix it
6. Verify the service
7. Monitor after recovery

This structured approach is what interviewers are looking for.

⭐ Star this repository if you found it useful.

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=PreethamRaj9121&label=Repo%20Views&color=0e75b6&style=flat" />
</p>
