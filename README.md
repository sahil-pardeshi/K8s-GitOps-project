
## 🚀 Overview
[cite_start]Engineered a declarative CI/CD pipeline using **Argo CD** and **GitOps** principles to manage containerized applications on AWS[cite: 15, 16]. This project ensures high availability and system reliability through automated synchronization.

## 🛠️ Technical Stack
* [cite_start]**Cloud:** AWS (EKS, VPC, IAM) [cite: 9]
* [cite_start]**Orchestration:** Kubernetes [cite: 9, 17]
* [cite_start]**GitOps:** Argo CD [cite: 16]
* [cite_start]**Observability:** Prometheus & Grafana [cite: 9, 16]

## 📈 Key Achievements
* [cite_start]**99.9% Availability:** Guaranteed through active health checks and Kubernetes workload orchestration[cite: 17].
* [cite_start]**Real-time Monitoring:** Designed custom Grafana dashboards to visualize cluster health, CPU, and Memory usage[cite: 16].

## ⚠️ Challenges & Troubleshooting
* **Issue:** **ImagePullBackOff** errors in the EKS cluster.
  * **Cause:** The worker nodes lacked IAM permissions to pull images from the private ECR.
  * [cite_start]**Solution:** Updated the IAM Role policy to include `AmazonEC2ContainerRegistryReadOnly`[cite: 18].
* **Issue:** **OOMKilled** pods in Prometheus.
  * [cite_start]**Solution:** Implemented Resource Limits/Requests and adjusted data retention periods to optimize memory[cite: 18].

