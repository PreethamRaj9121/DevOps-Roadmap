# ☸️ Kubernetes Commands Cheat Sheet

A quick Kubernetes reference for DevOps Engineers, Cloud Engineers, and SREs.

---

# 📦 Pod Commands

## List Pods

```bash
kubectl get pods
```

## List Pods with Details

```bash
kubectl get pods -o wide
```

## Describe Pod

```bash
kubectl describe pod <pod-name>
```

## View Logs

```bash
kubectl logs <pod-name>
```

## Stream Logs

```bash
kubectl logs -f <pod-name>
```

## Access Pod Shell

```bash
kubectl exec -it <pod-name> -- bash
```

## Delete Pod

```bash
kubectl delete pod <pod-name>
```

---

# 🚀 Deployment Commands

## List Deployments

```bash
kubectl get deployments
```

## Create Deployment

```bash
kubectl create deployment nginx --image=nginx
```

## Apply YAML

```bash
kubectl apply -f deployment.yaml
```

## Scale Deployment

```bash
kubectl scale deployment nginx --replicas=5
```

## Restart Deployment

```bash
kubectl rollout restart deployment nginx
```

## Check Rollout Status

```bash
kubectl rollout status deployment nginx
```

## Rollback Deployment

```bash
kubectl rollout undo deployment nginx
```

---

# 🌐 Service Commands

## View Services

```bash
kubectl get svc
```

## Describe Service

```bash
kubectl describe svc <service-name>
```

## Delete Service

```bash
kubectl delete svc <service-name>
```

---

# 🖥️ Node Commands

## View Nodes

```bash
kubectl get nodes
```

## Detailed Node Information

```bash
kubectl describe node <node-name>
```

## Drain Node

```bash
kubectl drain <node-name> --ignore-daemonsets
```

## Uncordon Node

```bash
kubectl uncordon <node-name>
```

---

# 📊 Monitoring Commands

## Check Pod Resource Usage

```bash
kubectl top pods
```

## Check Node Resource Usage

```bash
kubectl top nodes
```

---

# 🔍 Troubleshooting Commands

## View Events

```bash
kubectl get events
```

## Sort Events

```bash
kubectl get events --sort-by=.metadata.creationTimestamp
```

## View Everything in Namespace

```bash
kubectl get all -n <namespace>
```

## View ConfigMaps

```bash
kubectl get configmaps
```

## View Secrets

```bash
kubectl get secrets
```

---

# 🚨 Kubernetes Troubleshooting Flow

## Step 1

Check Pod Status

```bash
kubectl get pods
```

## Step 2

Check Events

```bash
kubectl describe pod <pod-name>
```

## Step 3

Check Logs

```bash
kubectl logs <pod-name>
```

## Step 4

Check Services

```bash
kubectl get svc
```

## Step 5

Check Ingress

```bash
kubectl get ingress
```

## Step 6

Check Resource Usage

```bash
kubectl top pods
```

---

# 🎯 Must Know Commands For Interviews

```bash
kubectl get pods
kubectl logs <pod-name>
kubectl describe pod <pod-name>
kubectl exec -it <pod-name> -- bash
kubectl get svc
kubectl get nodes
kubectl top pods
kubectl rollout status deployment
kubectl rollout undo deployment
kubectl get events
```

---

# 💡 Common Interview Questions

### What is a Pod?

Smallest deployable unit in Kubernetes.

### Difference Between Deployment and StatefulSet?

Deployment → Stateless Apps

StatefulSet → Stateful Apps

### What Causes CrashLoopBackOff?

* Application crash
* Wrong configuration
* Missing environment variables
* Database connectivity issues

### What Causes ImagePullBackOff?

* Wrong image name
* Registry authentication issues
* Image not found

### Difference Between ConfigMap and Secret?

ConfigMap → Non-sensitive data

Secret → Sensitive data

---

⭐ Star this repository if it helped you.

📸 Follow @devops._raj for DevOps Interview Questions, Projects, Roadmaps & Career Tips.
