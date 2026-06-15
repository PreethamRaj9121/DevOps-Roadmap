# 🐧 Linux Cheat Sheet for DevOps Engineers

## 📂 Navigation Commands

```bash
pwd                 # Current directory
ls                  # List files
ls -la              # Detailed list with hidden files
cd /path            # Change directory
cd ..               # Move one level up
cd ~                # Home directory
```

---

## 📄 File Operations

```bash
touch file.txt      # Create file
cat file.txt        # View file
less file.txt       # View large file
head -10 file.txt   # First 10 lines
tail -10 file.txt   # Last 10 lines
tail -f app.log     # Monitor logs
cp file1 file2      # Copy file
mv old new          # Move/Rename file
rm file.txt         # Delete file
rm -rf folder       # Delete folder
```

---

## 🔍 Search Commands

```bash
grep "ERROR" app.log
grep -i "error" app.log
find /var/log -name "*.log"
which kubectl
locate nginx
```

---

## 👤 User Management

```bash
whoami
id
sudo su -
useradd devops
passwd username
usermod -aG sudo username
```

---

## 🔒 Permissions

```bash
chmod 755 script.sh
chmod +x script.sh
chown user:user file.txt
ls -l
```

---

## ⚙️ Process Management

```bash
ps -ef
top
htop
pgrep nginx
kill PID
kill -9 PID
```

---

## 💾 Memory Usage

```bash
free -m
vmstat
```

---

## 💽 Disk Usage

```bash
df -h
du -sh *
du -sh /var/log
```

---

## 🌐 Networking

```bash
ping google.com
curl https://google.com
wget https://example.com/file.zip
nslookup google.com
dig google.com
```

---

## 🔌 Port Troubleshooting

```bash
ss -tulnp
netstat -tulnp
lsof -i :8080
```

---

## 📋 Service Management

```bash
systemctl status nginx
systemctl start nginx
systemctl stop nginx
systemctl restart nginx
systemctl enable nginx
```

---

## 📜 Log Analysis

```bash
tail -f /var/log/syslog
journalctl -xe
journalctl -u nginx
```

---

## 📦 Package Management (Ubuntu)

```bash
apt update
apt upgrade
apt install nginx
apt remove nginx
```

---

## 📦 Package Management (RHEL/CentOS)

```bash
yum update
yum install nginx
dnf install nginx
```

---

## ☸️ Kubernetes Related Linux Commands

```bash
kubectl get pods
kubectl get nodes
kubectl logs pod-name
kubectl describe pod pod-name
kubectl exec -it pod-name -- bash
```

---

## 🐳 Docker Related Linux Commands

```bash
docker ps
docker images
docker logs container
docker exec -it container bash
docker system prune -a
```

---

## 🚀 Top 10 Commands Every DevOps Engineer Uses Daily

```bash
ls -la
cd
grep
tail -f
cat
ps -ef
top
df -h
free -m
systemctl status
```

---

# 🎯 Interview Questions

### What is the difference between grep and find?

* grep → Searches content inside files
* find → Searches files/directories

### Difference between top and ps?

* top → Real-time monitoring
* ps → Snapshot of running processes

### Difference between chmod and chown?

* chmod → Changes permissions
* chown → Changes ownership

### How do you check disk space?

```bash
df -h
```

### How do you check memory usage?

```bash
free -m
```

---

⭐ Star this repository if it helped you.

📸 Follow @devops._raj for DevOps Interview Questions, Projects, Roadmaps & Career Tips.

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=PreethamRaj9121&label=Repo%20Views&color=0e75b6&style=flat" />
</p>
