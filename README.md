
This repo shows how to use Vagrant to set up a local centos 7.1 based Docker environment. 
It also gives an example on how to integrate Vagrant and Ansible.

[bento centos 7.1 box](https://atlas.hashicorp.com/bento/boxes/centos-7.1) is used. Only VirtualBox provider is verified but it should work with other providers like Parallels and VMware.

### Requirements
* Vagrant 1.7.4
* VirtualBox 5

Other versions of Vagrant and VirtualBox have not been verified. But they should work.

### Getting Started

```
git clone https://github.com/bluesalt/vagrant-docker
cd vagrant-docker
vagrant up
vagrant ssh
sudo docker pull centos
sudo docker run -i -t --rm centos /bin/bash
```
