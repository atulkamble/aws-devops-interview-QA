**50 AWS/DevOps Mock Interview Questions and Answers**, grouped into relevant categories with high-quality responses — ideal for interviews or preparation sessions:

---

## ✅ SECTION 1: IAM & AWS Core (Q1–Q10)

### **Q1. What is the difference between IAM Role and IAM User?**

**A:** IAM User is a permanent identity with credentials, used by people. IAM Role is a temporary identity assumed by services or users for access.

---

### **Q2. How does IAM Policy work?**

**A:** JSON-based documents that define permissions. Attached to users, groups, or roles. Contains Effect, Action, Resource, and Conditions.

---

### **Q3. How do you secure access to S3 buckets?**

**A:** Use IAM policies, bucket policies, block public access settings, and enable server-side encryption (SSE-S3, SSE-KMS).

---

### **Q4. Explain the Shared Responsibility Model.**

**A:** AWS manages security **of** the cloud (hardware, networking); customers manage security **in** the cloud (data, configuration).

---

### **Q5. What is EC2 and how do you secure it?**

**A:** EC2 is a virtual server. Secure it using key pairs, security groups, NACLs, SSH access restrictions, and updates.

---

### **Q6. What is the difference between a Security Group and a Network ACL?**

**A:** Security Group is stateful (return traffic allowed automatically), NACL is stateless and works at subnet level.

---

### **Q7. What are the different types of load balancers in AWS?**

**A:** ALB (HTTP/HTTPS), NLB (TCP/UDP), CLB (legacy). ALB supports path-based routing, NLB offers high performance.

---

### **Q8. How do you monitor an EC2 instance?**

**A:** Use CloudWatch metrics (CPU, disk, network), create alarms, and enable detailed monitoring for 1-minute metrics.

---

### **Q9. What is an Elastic IP?**

**A:** A static IPv4 address that can be attached to EC2 instances. Useful for failover and consistent public IP.

---

### **Q10. What is AWS Auto Scaling Group?**

**A:** Automatically adjusts the number of EC2 instances based on policies (CPU, network, time-based).

---

## ✅ SECTION 2: CI/CD & DevOps (Q11–Q20)

### **Q11. What is CI/CD and why is it important?**

**A:** CI ensures code integration with testing. CD automates deployments. Speeds delivery and reduces bugs.

---

### **Q12. What are Jenkins pipelines?**

**A:** Declarative or scripted Groovy-based automation to define CI/CD workflows. Uses `Jenkinsfile`.

---

### **Q13. How do you integrate Git with Jenkins?**

**A:** Use Git plugin, connect repo via webhook or poll SCM. Configure pipeline to pull code.

---

### **Q14. What is the purpose of a build tool in DevOps?**

**A:** Tools like Maven, Gradle, or npm compile code, manage dependencies, and produce build artifacts.

---

### **Q15. What is Artifact Repository?**

**A:** Central store for build artifacts — e.g., Nexus, Artifactory, or AWS CodeArtifact.

---

### **Q16. How do you handle rollback in CI/CD?**

**A:** Keep previous deployments stored and scripts ready. Use CodeDeploy rollback or Jenkins pipeline logic.

---

### **Q17. How do you implement notifications in a pipeline?**

**A:** Use Slack, email, or SMS plugins/hooks. Integrate using Webhooks or SNS topics.

---

### **Q18. What is the role of AWS CodePipeline?**

**A:** Fully managed CI/CD service integrating with CodeBuild, CodeDeploy, GitHub, etc.

---

### **Q19. What’s the difference between Jenkins and GitHub Actions?**

**A:** Jenkins is self-hosted and plugin-rich. GitHub Actions is cloud-native, integrates natively with GitHub.

---

### **Q20. How do you run parallel jobs in Jenkins pipeline?**

**A:** Use `parallel` block in `Jenkinsfile` to define and run jobs concurrently.

---

## ✅ SECTION 3: Docker & Kubernetes (Q21–Q30)

### **Q21. What is Docker and why is it used?**

**A:** Docker is a containerization platform that packages apps with dependencies, ensuring consistency across environments.

---

### **Q22. Difference between Docker Image and Container?**

**A:** Image is a static template; container is a running instance of that image.

---

### **Q23. What is a Dockerfile?**

**A:** Script to build Docker images — defines base image, instructions, environment, ports, volumes.

---

### **Q24. What is the purpose of Docker Compose?**

**A:** Tool to run multi-container applications using `docker-compose.yml`.

---

### **Q25. What is Kubernetes?**

**A:** Open-source container orchestration platform to manage scaling, self-healing, and deployments.

---

### **Q26. Difference between Deployment and StatefulSet in K8s?**

**A:** Deployment is stateless; StatefulSet maintains identity and order for stateful apps.

---

### **Q27. How do you expose a Kubernetes service?**

**A:** Using `Service` type: ClusterIP, NodePort, LoadBalancer, or Ingress.

---

### **Q28. How do you monitor Kubernetes?**

**A:** Use Prometheus and Grafana, or AWS CloudWatch Container Insights, EFK stack.

---

### **Q29. What is Helm in Kubernetes?**

**A:** A package manager to install and manage Kubernetes applications via charts.

---

### **Q30. What is a ConfigMap and Secret in K8s?**

**A:** ConfigMap stores non-sensitive config; Secret stores sensitive info encoded in base64.

---

## ✅ SECTION 4: Infrastructure as Code (Q31–Q40)

### **Q31. What is Terraform?**

**A:** IaC tool to provision infrastructure using HCL. Works across AWS, Azure, GCP.

---

### **Q32. Difference between Terraform and CloudFormation?**

**A:** Terraform is multi-cloud, uses state files. CloudFormation is AWS-native, tightly integrated.

---

### **Q33. What is `terraform plan` and `terraform apply`?**

**A:** `plan` previews changes; `apply` provisions resources as per code.

---

### **Q34. What is a Terraform state file?**

**A:** Tracks resource mapping to avoid drift. Can be stored remotely (S3 + DynamoDB).

---

### **Q35. What is a Terraform module?**

**A:** A reusable set of Terraform resources defined in its own directory.

---

### **Q36. How do you prevent resource deletion in Terraform?**

**A:** Use `lifecycle { prevent_destroy = true }` in resource block.

---

### **Q37. What is Ansible and how is it different from Terraform?**

**A:** Ansible is configuration management (push-based); Terraform is provisioning (declarative).

---

### **Q38. What is Cloud-init in EC2?**

**A:** Script executed at first boot to install packages or configure services.

---

### **Q39. What’s the purpose of `terraform destroy`?**

**A:** It removes all resources defined in the code and tracked in state.

---

### **Q40. How do you use Workspaces in Terraform?**

**A:** Separate environments (dev, test, prod) using isolated state files.

---

## ✅ SECTION 5: Monitoring, Logging, and Scenarios (Q41–Q50)

### **Q41. How do you monitor AWS resources?**

**A:** Using CloudWatch (metrics, logs), CloudTrail (API activity), X-Ray (tracing), or external tools.

---

### **Q42. What is AWS CloudTrail?**

**A:** Records all API activity in AWS — useful for auditing and compliance.

---

### **Q43. What is the difference between CloudWatch and CloudTrail?**

**A:** CloudWatch = metrics/logs. CloudTrail = API call logging for governance/audits.

---

### **Q44. How do you implement centralized logging in AWS?**

**A:** Use CloudWatch Logs, ship logs from EC2/Lambda, or use ELK/EFK stacks.

---

### **Q45. What is blue/green deployment in AWS?**

**A:** Two environments: one live (blue), one idle (green). Traffic is switched to new version post-verification.

---

### **Q46. What is canary deployment?**

**A:** Gradually roll out changes to a small subset of users before full deployment.

---

### **Q47. What happens when you delete a CloudWatch alarm?**

**A:** The alarm is removed, but the metrics remain unless the monitored resource is deleted.

---

### **Q48. How do you handle secrets in DevOps?**

**A:** Use AWS Secrets Manager, SSM Parameter Store, or Vault. Never hardcode in code.

---

### **Q49. What is a bastion host?**

**A:** A secure EC2 instance used as a jump server to access instances in private subnets.

---

### **Q50. How do you ensure high availability in AWS architecture?**

**A:** Use multi-AZ deployments, ASG, load balancers, Route 53 failover, and S3 for durability.

---
