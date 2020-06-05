# Loadbalancer && dnsmasq

```
ansible-playbook -i inventory -l kubebalancer_nodes kubeadm.yml

```
# Docker 

```
ansible-playbook -i inventory docker.yml

```

# Install Kubeadm,Kubectl,Kubelet Binrary and pull docker images

```
ansible-playbook -i inventory -l kubeadm_nodes kubeadm.yml

```

# KUBE MASTERS
# This can be only be used once ( during first cluster init )
```
ansible-playbook -i inventory -l kubemaster_nodes kubeadm.yml  --tags init

```

# TODO
    - Add Worker Playbook