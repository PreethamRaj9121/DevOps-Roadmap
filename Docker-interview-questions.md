# 🐳 Docker Interview Questions Repository

If you're preparing for DevOps, Cloud, SRE, or Platform Engineering interviews, this repository contains frequently asked Docker interview questions and real-world scenarios.

⭐ Star this repository if it helps you.

---

# Table of Contents

* Docker Fundamentals
* Dockerfile Questions
* Container Questions
* Networking Questions
* Volumes Questions
* Docker Compose Questions
* Scenario-Based Questions
* Troubleshooting Questions

---

# Docker Fundamentals

## 1. What is Docker?

Docker is a containerization platform that packages applications and their dependencies into lightweight containers.

---

## 2. What is a Container?

A running instance of a Docker image.

Example:

```bash
docker run nginx
```

---

## 3. What is a Docker Image?

A read-only template used to create containers.

Think:

```text
Image = Blueprint

Container = Running House
```

---

## 4. Difference Between Virtual Machines and Containers

### Virtual Machine

* Includes Guest OS
* Higher resource usage

### Container

* Shares Host OS Kernel
* Lightweight
* Faster startup

---

## 5. What Happens When You Run?

```bash
docker run nginx
```

Docker:

1. Checks local image
2. Pulls image if missing
3. Creates container
4. Creates writable layer
5. Starts container process

---

# Dockerfile Questions

## 6. What is a Dockerfile?

A text file containing instructions to build images.

Example:

```dockerfile
FROM nginx
COPY . /usr/share/nginx/html
```

---

## 7. Difference Between CMD and ENTRYPOINT

### CMD

Provides default arguments.

```dockerfile
CMD ["python","app.py"]
```

Can be overridden.

---

### ENTRYPOINT

Defines main executable.

```dockerfile
ENTRYPOINT ["python"]
```

Usually not overridden.

---

## 8. Can CMD and ENTRYPOINT Be Used Together?

Yes.

```dockerfile
ENTRYPOINT ["python"]
CMD ["app.py"]
```

Result:

```bash
python app.py
```

---

## 9. Difference Between COPY and ADD

### COPY

Copies files.

### ADD

Copies files + supports URLs and extraction.

Preferred:

```dockerfile
COPY
```

---

# Container Questions

## 10. How Do You List Running Containers?

```bash
docker ps
```

---

## 11. List All Containers

```bash
docker ps -a
```

---

## 12. Access Running Container

```bash
docker exec -it container_id bash
```

---

## 13. View Logs

```bash
docker logs container_id
```

---

## 14. Stop Container

```bash
docker stop container_id
```

---

## 15. Remove Container

```bash
docker rm container_id
```

---

# Networking Questions

## 16. What is Docker Bridge Network?

Default Docker network.

Containers communicate using private IPs.

---

## 17. List Networks

```bash
docker network ls
```

---

## 18. Create Network

```bash
docker network create devops-net
```

---

## 19. Difference Between Bridge and Host Network

### Bridge

Container gets isolated network.

### Host

Container shares host network.

---

# Volumes Questions

## 20. Why Use Volumes?

Containers are ephemeral.

Volumes persist data.

---

## 21. Create Volume

```bash
docker volume create myvolume
```

---

## 22. List Volumes

```bash
docker volume ls
```

---

## 23. Inspect Volume

```bash
docker volume inspect myvolume
```

---

# Docker Compose Questions

## 24. What is Docker Compose?

Tool for managing multi-container applications.

---

## 25. Start Services

```bash
docker compose up -d
```

---

## 26. Stop Services

```bash
docker compose down
```

---

## 27. View Running Services

```bash
docker compose ps
```

---

# Scenario-Based Questions

## Scenario 1

Container keeps restarting.

What will you check?

### Answer

* Logs

```bash
docker logs container_id
```

* Entrypoint
* Application errors
* Environment variables

---

## Scenario 2

Application works locally but not inside container.

What will you check?

### Answer

* Port mappings
* Environment variables
* Network connectivity
* Missing dependencies

---

## Scenario 3

Container exits immediately.

What will you check?

### Answer

* Main process
* CMD
* ENTRYPOINT
* Logs

---

## Scenario 4

Container cannot connect to database.

### Check

* Network
* Firewall
* Credentials
* DNS Resolution

---

# Troubleshooting Questions

## High Disk Usage

Check:

```bash
docker system df
```

Clean:

```bash
docker system prune -a
```

---

## High Container CPU Usage

Check:

```bash
docker stats
```

---

## Image Build Failure

Check:

* Dockerfile
* Build context
* Dependencies

---

# Top Docker Commands

```bash
docker pull nginx
docker images
docker build -t myapp .
docker run -d nginx
docker ps
docker logs container_id
docker exec -it container_id bash
docker stop container_id
docker rm container_id
docker volume ls
docker network ls
docker compose up -d
docker system prune -a
```

---

# Real Interview Questions

1. Difference between CMD and ENTRYPOINT?
2. What happens when docker run executes?
3. Difference between Image and Container?
4. How do Docker volumes work?
5. How do containers communicate?
6. Difference between COPY and ADD?
7. How do you debug container failures?
8. Explain Docker networking.
9. How do you optimize Docker images?
10. What is a multi-stage build?

---

# Follow

⭐ Star this repository

👨‍💻 Follow on GitHub

📸 Follow @devops._raj for daily DevOps interview questions and career content.

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=PreethamRaj9121&label=Repo%20Views&color=0e75b6&style=flat" />
</p>
