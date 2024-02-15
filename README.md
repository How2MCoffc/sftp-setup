# How-To-Setup-FTP-Access

You need to be outside of any folder or file or  directory and You must Be in root user mode ``sudo -s`` or ``sudo su``.

# Create User:
```sudo useradd -d /var/www username```

# Set a Password:
```sudo passwd username```

# Set directory permission for the user:
```nano /etc/ssh/sshd_config```

# Paste the lines:
`subsystem sftp internal-sftp` (Ignore this line if it is already there in the file, just uncomment the exsisting line.)
`Match User username`
`   ChrootDirectory %h`
`   AllowTCPForwarding no`
`   X11Forwarding no`
`   ForceCommand internal-sftp`

# Image
![Image](https://github.com/How2MCoffc/sftp-setup/assets/148950446/036215e0-3976-49d9-9da1-879dff28139a)

# Set permission(important):
```sudo chown -R username:username /var/www/pterodactyl```
```sudo chmod -R 755 /var/www/pterodactyl```

# Restart the SSH:
```sudo service ssh restart```
```sudo systemctl restart sshd```



> [!NOTE]
> The Port `22` Shoud Be Opened In The Firewall.
