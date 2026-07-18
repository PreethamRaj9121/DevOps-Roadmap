# 🚨 DevOps Production Scenarios

Real-world production issues and how to troubleshoot them like a DevOps Engineer.

---

# Scenario 1

## Production is DOWN

CPU: 20%

Memory: Normal

Users can't log in.

### Troubleshooting Steps

### 1. Check Application Logs

```bash
kubectl logs <pod-name>
```

or

```bash
docker logs <container-name>
```

---

### 2. Verify Recent Deployments

- Jenkins
- GitHub Actions
- GitLab CI
- ArgoCD

---

### 3. Check Database Connectivity

Ensure the application can reach the database and credentials are valid.

---

### 4. Verify Authentication

Check:

- OAuth
- LDAP
- JWT
- Identity Provider
- Session Store

---

### 5. Check Load Balancer / Ingress

Verify:

- Service
- Ingress
- DNS
- SSL Certificate

---

## Common Root Causes

- Bad deployment
- Database outage
- Authentication failure
- Expired secrets
- DNS issues
- Ingress misconfiguration
- Network policies
- Third-party service outage

---

## Commands

```bash
kubectl get pods
kubectl logs <pod-name>
kubectl describe pod <pod-name>
kubectl get svc
kubectl get ingress
kubectl get events
kubectl top pods
kubectl top nodes
```

---

⭐ Follow **@devops._raj** for more DevOps interview questions and production scenarios.

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=PreethamRaj9121&label=Repo%20Views&color=0e75b6&style=flat" />
</p>
