### Demo Project:

Automate Nexus Deployment via Ansible

### Technologies used:

Ansible, Nexus, DigitalOcean, Java, Linux

### Project Description:

1- Create Server on EC2 Instance.

2- Write Ansible Playbook that creates Linux user for Nexus, configure server, installs and deploys Nexus and verifies that it is running successfully

### Usage instruction

###### Step 1: Create an ec2 instance with 2ram in aws

![iamge](images/Screenshot%202023-04-20%20at%2010.17.21%20pm.png)

###### Step 2: Update apt and install java 8

![iamge](images/Screenshot%202023-04-20%20at%205.11.27%20pm.png)

![iamge](images/Screenshot%202023-04-20%20at%205.19.22%20pm.png)

###### Step3: Download Nexus installer

![iamge](images/Screenshot%202023-04-20%20at%205.24.20%20pm.png)

###### Step4: Rename Nexus installer folder

![iamge](images/Screenshot%202023-04-20%20at%205.54.09%20pm.png)

###### Step5: Create a new nexus user and group, and change the owner of nexus folder to new owner

![iamge](images/Screenshot%202023-04-20%20at%207.38.46%20pm.png)

###### Step 6: Set run_as_user nexus

###### Step 7: Run nexus as new user nexus

###### Step 8: Checking the running status

![iamge](images/Screenshot%202023-04-20%20at%2010.25.14%20pm.png)

###### Step 9: Run the nexus.yaml

```
ansible-playbook -i hosts nexus.yaml
```
