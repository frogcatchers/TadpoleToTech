---
layout: page
title: Learning Paths
permalink: /learning-paths/
---

# My IT Learning Journey

Welcome to my organized learning documentation! I've structured my studies into focused learning paths to track progress and build knowledge systematically.

## 🐳 Docker & Containerization
Learn the fundamentals of containerization and Docker.
{% for post in site.docker %}
- **[{{ post.title }}]({{ post.url | relative_url }})** - {{ post.date | date: "%b %d, %Y" }}
  {% if post.excerpt %}<br>*{{ post.excerpt }}*{% endif %}
{% endfor %}

{% if site.docker.size == 0 %}
*Coming soon: Docker basics, container management, and Dockerfile creation*
{% endif %}

## ☸️ Kubernetes
Orchestrating containers at scale.
{% for post in site.kubernetes %}
- **[{{ post.title }}]({{ post.url | relative_url }})** - {{ post.date | date: "%b %d, %Y" }}
  {% if post.excerpt %}<br>*{{ post.excerpt }}*{% endif %}
{% endfor %}

{% if site.kubernetes.size == 0 %}
*Coming soon: K8s fundamentals, deployments, services, and cluster management*
{% endif %}

## 🔄 CI/CD Pipelines
Automating testing, building, and deployment.
{% for post in site.ci-cd %}
- **[{{ post.title }}]({{ post.url | relative_url }})** - {{ post.date | date: "%b %d, %Y" }}
  {% if post.excerpt %}<br>*{{ post.excerpt }}*{% endif %}
{% endfor %}

{% if site.ci-cd.size == 0 %}
*Coming soon: GitHub Actions, automated testing, and deployment strategies*
{% endif %}

## 🤗 AI & Hugging Face
Machine learning, natural language processing, and Hugging Face ecosystem.
{% for post in site.ai %}
- **[{{ post.title }}]({{ post.url | relative_url }})** - {{ post.date | date: "%b %d, %Y" }}
  {% if post.excerpt %}<br>*{{ post.excerpt }}*{% endif %}
{% endfor %}

{% if site.ai.size == 0 %}
*Coming soon: Transformers, model fine-tuning, Hugging Face Hub, and AI applications*
{% endif %}

## ⛓️ Blockchain
Distributed ledgers, smart contracts, and decentralized applications.
{% for post in site.blockchain %}
- **[{{ post.title }}]({{ post.url | relative_url }})** - {{ post.date | date: "%b %d, %Y" }}
  {% if post.excerpt %}<br>*{{ post.excerpt }}*{% endif %}
{% endfor %}

{% if site.blockchain.size == 0 %}
*Coming soon: Bitcoin fundamentals, Ethereum, smart contracts, and DeFi protocols*
{% endif %}

## ⚛️ Quantum Computing
Quantum algorithms, quantum programming, and quantum machine learning.
{% for post in site.quantum %}
- **[{{ post.title }}]({{ post.url | relative_url }})** - {{ post.date | date: "%b %d, %Y" }}
  {% if post.excerpt %}<br>*{{ post.excerpt }}*{% endif %}
{% endfor %}

{% if site.quantum.size == 0 %}
*Coming soon: Quantum gates, quantum circuits, Qiskit, and quantum algorithms*
{% endif %}

## 🛠️ Hands-On Projects
Real-world applications and practical implementations.
{% for post in site.projects %}
- **[{{ post.title }}]({{ post.url | relative_url }})** - {{ post.date | date: "%b %d, %Y" }}
  {% if post.excerpt %}<br>*{{ post.excerpt }}*{% endif %}
{% endfor %}

{% if site.projects.size == 0 %}
*Coming soon: Full-stack applications, infrastructure projects, and automation scripts*
{% endif %}

---

## Progress Overview
- **Docker Posts:** {{ site.docker.size }}
- **Kubernetes Posts:** {{ site.kubernetes.size }}  
- **CI/CD Posts:** {{ site.ci-cd.size }}
- **AI Posts:** {{ site.ai.size }}
- **Blockchain Posts:** {{ site.blockchain.size }}
- **Quantum Posts:** {{ site.quantum.size }}
- **Project Posts:** {{ site.projects.size }}

*Last updated: {{ site.time | date: "%B %d, %Y" }}*
