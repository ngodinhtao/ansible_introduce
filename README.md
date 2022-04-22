# ansible_introduce

Ansible is an agentless automation tool that you install on a control node. From the control node, Ansible manages machines and other devices remotely (by default, over the SSH protocol). 

![alt text](https://user-images.githubusercontent.com/17456175/164676997-49d02abf-c3a9-43f7-b8dd-4ccc9d10cae8.png)

## Intallation
# On Ubuntu
apt-add-repository -y ppa:ansible/ansible
apt-get update
apt-get install -y ansible
# On centos
yum install epel-release
yum install ansible

# On Window
No, Ansible can only manage Windows hosts. Ansible cannot run on a Windows host natively, though it can run under the Windows Subsystem for Linux (WSL).

# On MacOs
The preferred way to install Ansible on a Mac is with pip
If you are installing on macOS Mavericks (10.9), you may encounter some noise from your compiler. A workaround is to do the following:

$ CFLAGS=-Qunused-arguments CPPFLAGS=-Qunused-arguments pip install --user ansible
