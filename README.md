# ☸️ Kubernetes Infrastructure & Applications Portfolio

This repository contains a collection of Kubernetes manifests (YAML files) for deploying infrastructure and applications on a K8s cluster. The projects demonstrate various cluster management capabilities, ranging from simple stateless deployments to stateful applications with persistent storage and system monitoring.

## 🏗️ Architecture Overview

The infrastructure utilizes the following Kubernetes objects:
* **Deployments:** Managing pod lifecycles and ensuring high availability.
* **Services:** Exposing applications via `NodePort` and `ClusterIP`.
* **Persistence:** Implementing **Persistent Volume Claims (PVC)** for data durability (Nextcloud, PostgreSQL).
* **Observability:** Real-time monitoring of cluster resources (CPU, RAM, Network).

## 🚀 Deployment Catalog

| Application | Configuration File | Key Features |
| :--- | :--- | :--- |
| **Nextcloud** | `nextcloud.yaml` | Private Cloud, PVC Integration, Environment Variables |
| **Netdata** | `netdata.yaml` | System Monitoring, Real-time Dashboard, Node Metrics |
| **Planka** | `planka.yaml` | Multi-container Deployment, PostgreSQL DB Backend |
| **Super Mario** | `mario.yaml` | Web UI, Load Balancing Demo |
| **2048 Game** | `game-2048.yaml` | Logic Game Deployment |
| **Animals Portfolio** | `animals-portfolio.yaml` | Custom Frontend Deployment |

## 🛠️ Usage Instructions

To apply all configurations to your cluster at once:

```bash
# Apply all YAML files in the current directory
kubectl apply -f .
