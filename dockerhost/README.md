# ansible-example: Dockerhost
Ansible example for educational purposes.

Prerequisites:

	- 2x Ubuntu 18.04 server
	- user bob added to sudoers file (NOPASSWD)
		- 'sudo visudo'
	- ssh pub key needs to be added to the authorized keys within the machine
		- 'ssh-copy-id'

To run this example, you need two linux VM's. Check the 'hosts' file within and change the Ip-adresses. Also, change the ssh username. The user running within the linux machines needs to be a sudo user. 

> In later examples we can use a ansible-vault to supply the root password. Or we can delete the initial user when provisioning is done. All food for thought, and dont forget this is just a simple example playbook to set up a 'dockerhost' on Ubuntu 18.04 server.

To run the playbook:

```bash
ansible-playbook site.yml -i hosts -v
```
