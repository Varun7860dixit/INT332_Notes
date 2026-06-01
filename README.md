#  Mastering DevOps: Virtualization, Containerization & CI/CD Pipelines

---

## 🎯 Repository Mission & Overview

Welcome to **DOCKER-LEARNING**. This repository serves as an end-to-end engineered record of modern DevOps methodologies spanning **OS-Level Virtualization**, **Microservices Orchestration**, **Build Automation**, and **Continuous Integration (CI/CD)** engines. 

This space tracks theoretical milestones alongside practical shell checkpoints, custom docker scripts, and live automation pipelines, organized cleanly by academic units.

---

## 📂 Repository Architecture & Syllabus Mapping

The workspace is cleanly divided into 6 fundamental core units. Navigate into any unit folder to view standalone `README.md` technical specs, logs, and laboratory screenshots.

### 🏗️ Part 1: Virtualization & Container Mechanics

| Unit Link | Module Name | Core Engineering Focus & Deliverables |
| :--- | :--- | :--- |
| [**`📁 Unit_01`**](./UNIT-1) | **Basics of DevOps Infrastructure** | Linux kernel mechanics, Namespaces process isolation, Control Groups (`cgroups`) resource limits, and Docker Engine CLI basics. |
| [**`📁 Unit_02`**](./UNIT-2) | **Image Building & Management** | Writing optimized custom `Dockerfiles`, multi-layer filesystem structures, bridge networking, host port mapping, and volume storage persistence. |
| [**`📁 Unit_03`**](./UNIT-3) | **Microservices with Docker Compose** | Monolith decomposition architectures, multi-container YAML schemes, `build` vs `image` environments, and service initialization dependencies (`depends_on`). |

### 🚀 Part 2: Enterprise Build Automation & CI/CD Pipelines

| Unit Link | Module Name | Core Engineering Focus & Deliverables |
| :--- | :--- | :--- |
| [**`📁 Unit_04`**](./UNIT-4) | **Maven Build Automation** | Project Object Model (`pom.xml`) lifecycles, transitive dependency mapping, `mvnw` wrapper setups, and automated application containerization. |
| [**`📁 Unit_05`**](./UNIT-5) | **Continuous Integration with GitHub Actions** | Event-driven cloud workflows, declarative YAML runner matrices, dependency build caching, and automated image publishing to Docker Hub/GHCR. |
| [**`📁 Unit_06`**](./UNIT-6) | **CI/CD with Jenkins** | Distributed Controller-Agent nodes, Pipeline-as-Code setups via `Jenkinsfile`, GitHub webhooks automation, and production deployment flows. |

---

## ⚡ Production-Ready Command Playground
```text
🚀 THE DevOps PIPELINE FLOW:
 [ Code Push ] ──► [ GitHub Actions / Jenkins ] ──► [ Maven Compile ] ──► [ Docker Build ] ──► [ Registry Push ]
```

Examples of the complex multi-parameter configurations implemented and mastered throughout this repository:

### 🐳 1. Dynamic Container Provisioning with Storage & Network Isolation
```bash
docker run -d \
  --name scalable-api-runtime \
  --network custom-isolated-bridge \
  -p 8080:80 \
  -e APP_ENV=production \
  -v persistence_volume:/app/data \
  --memory="512m" --cpus="1.0" \
  ubuntu:latest
```
### 📦 2. Executing Standardized Build Lifecycle Streams
```bash
# Compile, run unit tests, and package application bypassing localized Maven variations
./mvnw clean package
```
### 🛠️ 3. Containerized Runtime Interrogation
```bash
# Audit immutable historical file layer footprints inside custom built images
docker history my-custom-app:latest

# Extract raw network metadata configurations and environment parameters
docker inspect scalable-api-runtime
```

### 🐙 4. GitHub Actions: Declarative Automated Matrix Trigger
```bash
# A snippet of the high-performance matrix strategy implemented in Unit 5
strategy:
  matrix:
    os: [ubuntu-latest, windows-latest]
    java-version: [17, 21]
```
### 🤖 5. Jenkinsfile: Multi-Stage Pipeline Execution Core
```bash
// Structural breakdown of the automated workflow engineered in Unit 6
stage('Build & Push Stack') {
    steps {
        sh 'docker build -t vansharora/prod-api:${BUILD_NUMBER} .'
        sh 'docker push vansharora/prod-api:${BUILD_NUMBER}'
    }
}
```
