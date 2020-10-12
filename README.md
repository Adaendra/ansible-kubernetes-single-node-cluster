# Ansible-kubernetes-single-node-cluster
Ansible scripts to generate a Kubernetes Single Node Cluster

This playbook was made for Ubuntu 18.04

<br/>

## Playbooks
### Create Playbook
Playbook to create the Kubernetes single node cluster with Docker.

*Command:*
```
ansible-playbook create-playboook.yml -i hosts
```


### Delete Playbook
Playbook to remove the Kubernetes cluster then remove packages of Kubernetes and Docker.

*Command:*
```
ansible-playbook delete-playboook.yml -i hosts
```

<br/>

## Roles
### Principals
* **delete_docker**\
To delete Docker from the machine.
* **reset_cluster**\
To reset the Kubernetes cluster.

### Additionnals
* **herm**\
Role to install Helm to help for Kubernetes deployments.
* **k8s_dashboard**\
To Install the Kubernetes Dashboard.