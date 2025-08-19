# 1. Introduction to Kubernetes

## Index
- [Overview](#overview)
- [Why Kubernetes](#why-kubernetes)
- [What Kubernetes Provides](#what-kubernetes-provides)
- [What Kubernetes is Not](#what-kubernetes-is-not)

---

## Overview
- Kubernetes (K8s) is an open-source container orchestration platform.
- Automates deployment, scaling, and management of containerized applications.
- Initially developed by Google; donated to CNCF (Cloud Native Computing Foundation).

---

## Why Kubernetes
- Containers are a good way to package and run applications, but in production they need **management** and **high availability**.  
- Kubernetes ensures no downtime by restarting or replacing failed containers automatically.  
- Provides a **framework to run distributed systems resiliently**, handling:  
  - Scaling  
  - Failover  
  - Deployment patterns (e.g., canary deployments)  

---

## What Kubernetes Provides
- **Service Discovery & Load Balancing** → Expose containers via DNS/IP, distribute traffic evenly.  
- **Storage Orchestration** → Mount storage from local or cloud providers automatically.  
- **Automated Rollouts & Rollbacks** → Ensure actual state matches desired state at a controlled pace.  
- **Automatic Bin Packing** → Efficiently schedule containers on cluster nodes based on CPU/RAM requirements.  
- **Self-Healing** → Restart, replace, or remove unhealthy containers.  
- **Secret & Config Management** → Store/manage sensitive data (passwords, tokens, SSH keys) securely.  
- **Batch Execution** → Manage batch jobs and CI workloads.  
- **Horizontal Scaling** → Scale apps manually or automatically (e.g., CPU usage).  
- **IPv4/IPv6 Dual Stack** → Support both address families.  
- **Designed for Extensibility** → Add features without modifying core source code.  

---

## What Kubernetes is Not
- **Not a traditional PaaS** → It provides building blocks, not a monolithic solution.  
- **Not limited to specific workloads** → Supports stateless, stateful, and data-processing workloads.  
- **Does not build/deploy source code** → CI/CD is external.  
- **Does not provide app-level services** → (e.g., middleware, databases, caches, message queues).  
- **Does not dictate logging/monitoring/alerting** → Integrations are optional.  
- **Does not enforce a config language** → Uses a declarative API that tools can target. Meaning you don't need to provide complete instructions instead you can provide what state you wanted in declarative way like usin YAML.  
- **Not a machine management system** → Doesn’t handle hardware-level maintenance or provisioning.  
- **Not just an orchestrator** → Instead of centralized workflows, Kubernetes uses **independent control processes** that continuously drive the cluster towards the desired state.  

---

