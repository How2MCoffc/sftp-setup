# How-To-Setup-FTP-Access

1. You should be outside of any folder / file / directory and You need Be in root user ``sudo -s``. 
2. You need to go in a file .So run `nano /etc/ssh/sshd_config`.
3. You need to go down and find `PermitRootLogin` and `PasswordAuthentication` make them Yes.

# Image
![image](https://github.com/How2MCoffc/sftp-setup/assets/148950446/cf97d586-fb23-47c8-9833-05d3a7768f51)

5. Then run `sudo systemctl restart sshd` So that the changes take place.

> [!NOTE]
> The Port `22` Shoud Be Open In The Firewall.
