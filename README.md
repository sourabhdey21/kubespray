# kubespray
Create Production Ready Kubernetes Cluster Using Ansible
Are you looking for an easy guide on how to install Kubernetes (k8s) using kubespray?

The step-by-step guide on this page will show you how to install Kubernetes Cluster using kubespray on linux systems.

Kubespray is a free and open-source tool that provide ansible playbooks to deploy and manage Kubernetes clusters. It is designed to simplify the installation process of Kubernetes clusters across multiple nodes, allowing users to deploy and manage a production-ready Kubernetes cluster quickly and easily.

It supports a range of operating systems, including Ubuntu, CentOS, Rocky Linux and Red Hat Enterprise Linux, and it can deploy Kubernetes on a variety of platforms, including bare metal, public cloud, and private cloud.

# In this guide, we are using the following lab,

Ansible Node (Kubespray Node): Minimal installed Ubuntu 22.04 LTS (192.168.1.240)
3 Controller Nodes: Minimal Installed Rocky Linux 9 (192.168.1.241/242/243)
2 Worker Nodes: Minimal Installed Rocky Linux 9 (192.168.1.244/245)

Minimum system requirements for kubespray

Master Nodes: 1500 MB RAM, 2 CPU and 20 GB free disk space

Worker Nodes: 1024 MB, 2 CPU, 20 GB free disk space

Ansible Node: 1024 MB, 1CPU and 20 GB disk space

Internet connectivity on each node

Regular with sudo admin rights

# Without any further delay, let’s deep dive into the installation steps,

