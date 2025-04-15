# Ansible Code Along
## Launch EC2 Instance
### Ansible Controller & Taget Node
Launch two blank EC2 instance running Ubuntu Server: 22.04 - t2.micro - sg with port 22(ssh). Title one Controller and the other Target

![EC2](./Images/launchcon.png)

## SSH into Controller Node
![SSH](./Images/loginssh.png)
- Connect using ssh client (gitbash)

### Check Python , Update and Upgrade
![Python Update](./Images/pythonupdate.png)

- Check that Python3 is running (needed for Ansible)
- Update packages
- Upgrade packages
  
### Install Ansible & Configure Permission
![Ansi](./Images/installansi.png)

  - Install Ansible using: sudo apt install ansible -y.
  - Check Version(ansible --version)
  
![Perm](./Images/perm.png)

- cd into ssh folder.
- create a aws private key file (must match target node key).
- use chmod400 to give super user read permission, enabling user ability to view the contents of the file (needed to ssh)
  
![Perm](./Images/ansihosts.png)

- cd into ansible folder
- edit hosts file
- edit new inventory called web and add target node
![Perm](./Images/web.png)

### Test connection
![Ping](./Images/ping.png)

- once saved test connection using sudo ansible web -m ping

### Ansible commands
![Update](./Images/update.png)
![Upgrade](./Images/upgrade.png)
