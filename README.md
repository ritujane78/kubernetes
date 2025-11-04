# ☸️ Kubernetes Basics

This repository contains **YAML configuration files** demonstrating essential Kubernetes concepts, including **Pods, Deployments, Services, ConfigMaps, Volumes, and more**. 

---

## 📘 Overview

The examples here focus on:
- Creating and managing **Pods**, **ReplicaSets**, and **Deployments**
- Exposing applications through **ClusterIP**, **NodePort**, and **LoadBalancer Services**
- Managing configuration and data using **ConfigMaps**, **Secrets**, and **Volumes**
- Scaling and observing workloads using **kubectl** commands
- Understanding how Kubernetes manages **containerized applications** in clusters

---

## ⚙️ Common Commands

### **Check Cluster Nodes**
```bash
kubectl get nodes
```

### **Deploy a Resource**
```bash
kubectl apply -f <filename>.yaml
```

### **View Pods and Services**
```bash
kubectl get pods
kubectl get svc
```

### **Describe a Resource**
```bash
kubectl describe pod <pod-name>
```

### **Delete a Resource**
```bash
kubectl delete -f <filename>.yaml
```

---

## 🧩 Key Concepts Demonstrated

| Concept | YAML Example | Description |
|----------|---------------|-------------|
| **Pod** | `pod.yaml` | Smallest deployable unit in Kubernetes |
| **Deployment** | `deployment.yaml` | Manages Pods and ensures desired replica count |
| **Service** | `service.yaml` | Exposes Pods to internal or external traffic |
| **ConfigMap** | `configmap.yaml` | Stores configuration data for Pods |
| **Persistent Volume** | `pv.yaml`, `pvc.yaml` | Manages data storage independent of Pod lifecycle |
| **Secrets** | `secret.yaml` | Stores sensitive data securely |
| **Namespace** | `namespace.yaml` | Provides isolation between environments |

---

## 🔍 Monitoring and Scaling

### **View Resource Usage**
```bash
kubectl top pods
kubectl top nodes
```

### **Scale a Deployment**
```bash
kubectl scale deployment <deployment-name> --replicas=<number>
```

### **Access a Pod Shell**
```bash
kubectl exec -it <pod-name> -- /bin/bash
```

---

## 🌐 Example Scenarios

- Deploying a sample web server using `nginx` or `httpd`
- Exposing it externally using a **NodePort Service**
- Managing app configuration through a **ConfigMap**
- Persisting data using **PersistentVolumes**
- Observing resource usage and scaling deployments

---

## 📚 References

- [Kubernetes Documentation](https://kubernetes.io/docs/)
- [kubectl Command Reference](https://kubernetes.io/docs/reference/kubectl/overview/)
- [TJ Adams — Kubernetes Fast Track (Udemy)](https://www.udemy.com/course/kubernetes-fast-track/?referralCode=82645BCEB61A64C1CC87)

---

## 🧠 Author

**Ritu Bafna**  
MSc Advanced Computer Science — University of Liverpool  
