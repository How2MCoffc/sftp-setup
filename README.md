# How-To-Setup-FTP-Access

1. You should be outside of any folder / file / directory and You need Be in root user ``sudo -s``. 
2. You need to go in a file .So run `nano /etc/ssh/sshd_config`.
3. You need to go down and find `PermitRootLogin` and `PasswordAuthentication` make them Yes.

# Image
![image]([https://github.com/CoconutGamer/How-To-Setup-FTP-Access/assets/154960261/7c187de7-aba0-4cb0-8f1d-ca7b5d854535](https://media.discordapp.net/attachments/942694327069577246/1207218554496356383/304402490-7c187de7-aba0-4cb0-8f1d-ca7b5d854535.png?ex=65ded8e4&is=65cc63e4&hm=eaad15898c10c453580e1491a4d8f9cfd517e1e55d1ced021069f04037a63b8f&=&format=webp&quality=lossless&width=939&height=559)https://media.discordapp.net/attachments/942694327069577246/1207218554496356383/304402490-7c187de7-aba0-4cb0-8f1d-ca7b5d854535.png?ex=65ded8e4&is=65cc63e4&hm=eaad15898c10c453580e1491a4d8f9cfd517e1e55d1ced021069f04037a63b8f&=&format=webp&quality=lossless&width=939&height=559)

5. Then run `sudo systemctl restart sshd` So that the changes take place.

> [!NOTE]
> The Port `22` Shoud Be Open In The Firewall.
