
# Vagrantfile and Scripts to Automate Kubernetes Setup using Kubeadm [Practice Environment for CKA/CKAD and CKS Exams]

A fully automated setup for CKA, CKAD, and CKS practice labs is tested on the following systems:

- Windows
- Ubuntu Desktop
- Mac Intel-based systems

## Setup Prerequisites

- A working Vagrant setup using Vagrant + VirtualBox

## Documentation

Current k8s version for CKA, CKAD, and CKS exam: 1.30.X 

The setup is updated with 1.30.X cluster version.

## Prerequisites

1. Working Vagrant setup
2. 8 Gig + RAM workstation as the Vms use 2 vCPUS and 4+ GB RAM
## Bring Up the Cluster

To provision the cluster, execute the following commands.

```shell
git clone https://github.com/rchidana/Two-Node-K8s-Cluster-kubeadm.git
cd Two-Node-K8s-Cluster-kubeadm
vagrant up
```
## To login to control-plane
```
vagrant status
vagrant ssh controlplane
```

## To shutdown the cluster,

```shell
vagrant halt
```

## To restart the cluster,

```shell
vagrant up
```

## To destroy the cluster,

```shell
vagrant destroy -f
```

