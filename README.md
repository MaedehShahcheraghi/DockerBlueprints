# 🐳 Docker Blueprints

![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=flat-square&logo=docker&logoColor=white)
![.NET](https://img.shields.io/badge/.NET_8-Optimized-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-Alpine-009639?style=flat-square&logo=nginx&logoColor=white)

> A clean, curated collection of production-ready and highly optimized Dockerfiles.

This repository serves as a practical boilerplate archive for containerizing modern applications, with a strict focus on **security**, **minimal image size**, and **CI/CD efficiency**.

## ✨ Core Principles

* **🔒 Rootless Security:** Containers run using restricted, non-root accounts to mitigate breakout vulnerabilities.
* **⚡ Multi-Stage Builds:** Separating the build environment from the runtime for ultra-lightweight production images.
* **📦 Layer Caching:** Strategic ordering of operations (e.g., copying `.csproj` files first) to optimize build speed.
* **🩺 Active Monitoring:** Custom `HEALTHCHECK` configurations tailored for orchestration platforms.

## 📁 Repository Structure

```text
.
├── nginx-static/
│   ├── Dockerfile          # Optimized Alpine-slim Nginx server
│   └── README.md           # Configuration details
│
└── dotnet-api/
    ├── Dockerfile          # Multi-stage, rootless .NET 8 blueprint
    └── README.md           # Build and runtime breakdown
