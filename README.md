# k3s Hello World

## Overview

This project automates the installation of a single-node Kubernetes (k3s) cluster using Ansible and deploys a Hello World Nginx application.

## Project Structure

```
k3s-challenge/
├── ansible/
│   ├── install-k3s.yml
│   └── inventory
├── k8s/
│   ├── deployment.yaml
│   └── service.yaml
└── README.md
```

## Features

- Automated k3s installation using Ansible
- Single-node Kubernetes cluster
- Nginx Hello World deployment
- NodePort Service
- GitHub Actions CI/CD

## Deployment

```bash
ansible-playbook -i ansible/inventory ansible/install-k3s.yml
```

Deploy application:

```bash
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
```

