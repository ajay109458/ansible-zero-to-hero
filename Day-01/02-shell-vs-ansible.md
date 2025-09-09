# Comparison with Shell Scripting

- Shell Scripting works only for Linux.

- Becomes complex and less readable(for non-experts) as the script size goes high.

- Idempotence and predictability

When the system is in the state your playbook describes Ansible does not change anything, even if the playbook runs multiple times.

for example, run the below shell script twice and you will notice the script will fail. Which means shell scripting is not idempotent in nature.

```
#/bin/bash

set -e 

mkdir test-demo
echo "hi"
```

- Scalability and flexibility

Easily and quickly scale the systems you automate through a modular design that supports a large range of operating systems, cloud platforms, and network devices.

### Issues with Python 
1. Python knowledge
2. Maintenance
3. Login to each machine (paramiko/fabric)

### Ansible 
1. Read inventory to understand the machine.
2. Execute on the machine.
3. Doesn't require strong configuraiton management.

Ansible is not good if you have to trigger the automation. 


Ansible --> Provisioning --> Terraform or Ansible. 

Core Skill of Terraform -> Provisioning Infrastructure 
Ansible ---> Config Management 

### Command 
```
pip install ansible
```
