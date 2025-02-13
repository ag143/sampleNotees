# DevOps Notes 🛠️

A single-page DevOps knowledge base with **tabs, collapsible sections, and interactive diagrams**.

## 📌 Quick Links
- 🚀 [Terraform](#terraform)
- 🐳 [Kubernetes](#kubernetes)
- ⚙️ [CI/CD](#ci-cd)

---

## 🌍 **DevOps Tools**

=== ":cloud: Terraform"
    ??? note "Click to Expand - Terraform Basics"
        - 🏗 **Infrastructure as Code (IaC)**
        - 📦 **Modules, State Management**
        - 🔄 **Terraform Cloud & Remote State**
    
    ```terraform
    resource "aws_instance" "web" {
      ami           = "ami-123456"
      instance_type = "t2.micro"
    }
    ```

=== ":whale: Kubernetes"
    ??? tip "Click to Expand - Kubernetes Essentials"
        - 🚀 **Pods, Deployments, Services**
        - 🎭 **Helm & Operators**
    
    ```yaml
    apiVersion: apps/v1
    kind: Deployment
    metadata:
      name: my-app
    spec:
      replicas: 3
      selector:
        matchLabels:
          app: my-app
      template:
        metadata:
          labels:
            app: my-app
        spec:
          containers:
            - name: my-container
              image: nginx
    ```

=== ":gear: CI/CD"
    ??? question "Click to Expand - CI/CD Pipelines"
        - ✅ **GitHub Actions, Jenkins, GitLab CI**
        - 🔄 **ArgoCD, Spinnaker**
    
    ```yaml
    name: CI Pipeline
    on: [push]
    jobs:
      build:
        runs-on: ubuntu-latest
        steps:
          - name: Checkout Code
            uses: actions
