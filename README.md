# How-To-Setup-FTP-Access

1. You should be outside of any folder or file or  directory and You must Be in root user mode ``sudo -s`` or ``sudo su``. 
2. You need to open a file localted in `/etc/ssh/`. So run `nano /etc/ssh/sshd_config`.
3. You need to go down and find `PermitRootLogin` and `PasswordAuthentication`. Set their property Yes.

# Image
![image](https://github.com/How2MCoffc/sftp-setup/assets/148950446/cf97d586-fb23-47c8-9833-05d3a7768f51)

5. Then run `sudo systemctl restart sshd` So that the changes take place.

> [!NOTE]
> The Port `22` Shoud Be Opened In The Firewall.
