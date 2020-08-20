# vagrant-box-bionic64-kind
A Vagrantbox ready  for running local Kubernetes clusters with [Kind](https://kind.sigs.k8s.io/) .

## Description
This repository contains everything needed to build the bionic64-kind vagrant box. Currently only a box for the Virtualbox provider is built.

This box is based on the hashicorp/bionic64, a standard Ubuntu 18.04 LTS 64-bit  provided by Hashicorp.

The next tools are included in the box:
* kind
* docker
* kubectl


## Usage
You can use the base box like any other base box. 

Clone this repo:
```
$ git clone git@github.com:galvarado/vagrant-box-bionic64-kind.git```
```

Create the box:
```
$ vagrant up
```

Login with ssh:
```
$ vagrant ssh
```

Get the k8s details with kubectl:

```
$ kubectl cluster-info
Kubernetes master is running at https://127.0.0.1:46157
KubeDNS is running at https://127.0.0.1:46157/api/v1/namespaces/kube-system/services/kube-dns:dns/proxy

To further debug and diagnose cluster problems, use 'kubectl cluster-info dump'.
```

[PENDING]

## Changelog
You can find the changelog [here](CHANGELOG.md)
