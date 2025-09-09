# Introduction to Ansible

## What is Ansible ?

Ansible is an open source IT automation engine that automates 
- provisioning 
- configuration management
- application deployment (CI/CD)
- orchestration
- Network Automation+ (Cisco/F5 - 

and many other IT processes. It is free to use, and the project benefits from the experience and intelligence of its thousands of contributors.

## How Ansible works ?

Ansible is agentless in nature, which means you don't need install any software on the manage nodes.

For automating Linux and Windows, Ansible connects to managed nodes and pushes out small programs—called Ansible modules—to them. These programs are written to be resource models of the desired state of the system. Ansible then executes these modules (over SSH by default), and removes them when finished. These modules are designed to be idempotent when possible, so that they only make changes to a system when necessary.

For automating network devices and other IT appliances where modules cannot be executed, Ansible runs on the control node. Since Ansible is agentless, it can still communicate with devices without requiring an application or service to be installed on the managed node.

## Example 
There are 4 Linux physical machines and one Windows Machine. 

System Admins need to perform the following operations manually or scripts
1. Up to date (supported)
2. open SSH/ Wget / CURL / Shared
3. Application dependency -> e.g. web server, java, application are installed on these machines.
4. Maintenance of these servers. 

Scripts:
1. Same script won't work on the windows.
2. Same script don't work on different version of the linux OS.

Then came some configuration management looks like:
1. Puppet
2. Chef
3. Salt
4. Ansible

### Puppet and Chef 
- Very popular 6-7 years backs.
- Learning curve was high (e.g. Rubby)
- Agent need to be installed on each machine.

### Ansbile
- You only need to know YAML

  <img width="786" height="385" alt="image" src="https://github.com/user-attachments/assets/381d9f6d-6cb4-42f4-8421-5f746d83f7f5" />

