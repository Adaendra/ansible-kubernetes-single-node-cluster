# Ansible-kubernetes-single-node-cluster
Ansible scripts to generate a Kubernetes Single Node Cluster

This playbook was made for Ubuntu 18.04

<br/>

## Playbooks
### Create Playbook
Playbook to create the Kubernetes single node cluster with Docker.

*Command to execute from the ansible folder:*
```
ansible-playbook create-playboook.yml -i inventory/hosts
```


### Delete Playbook
Playbook to remove the Kubernetes cluster then remove packages of Kubernetes and Docker.

*Command to execute from the ansible folder:*
```
ansible-playbook delete-playboook.yml -i inventory/hosts
```

<br/>

## Roles
### Used
* **delete_docker**\
To delete Docker from the machine.
* **delete_k8s**\
To delete Kubernetes from the machine
* **install_calico**\
To install Calico
* **install_docker**\
To install Docker.
* **install_k8s**\
To install kubernetes packages.
* **k8s_cluster**\
To create the Kubernetes cluster.
* **reset_cluster**\
To reset the Kubernetes cluster.

### Additionnals
* **helm**\
To install Helm for helping for Kubernetes deployments.
* **k8s_dashboard**\
To Install the Kubernetes Dashboard.