# Project to practice for the future.

This project will be separated into 2 folders.

- ansible
- teraform

_any study information will be located in its respective folder_

## Teraform Project Requirements

Layer-00 (directory)

- Deploy a VPC
- Deploy a IGW
- Deploy at least one NGW
- Deploy at least one public subnet
- Deploy at least one private subnet
- Use correct Routing
- Use at least one ingress Security Group
- Use at least one egress Security Group

Layer-01 (directory)

- Declare at lease one IAM profile

Layer-02 (directory)

- Deploy an instance with only a private IP
- Deploy one instance with a public IP using the VPN AMI
- Configure the VPN
  
## Ansible Project
Ansible Project
* Hostname is changes to <employee-ID> (can be whatever you want since you don't have yet :) )
  * The employee ID should be passed as a variable
  * Ansible enforces lowercase
* Add at least one additional volume using the "disk management role" (don't worry about this i'll provide context for this later)
* Configure Red Hat repository using the "Repository Management Role"
* Install the terraform binary
* Disable ansible host-key checking
* Enable ansible Logging
  * Permissions should be set so any user running ansible will log their ansible execution
* Update `logrotate` behavior for `/var/log/rotate`
  * update every 4 hours
  * archive logs older than 24 hours
  * Append the prefix `archive` to archived logs
  * Move the archived logs to the newly attached volume