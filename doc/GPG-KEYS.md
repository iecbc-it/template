#### Configure GPG key if they are requried
- Install https://gpgtools.org/ 
- Generate a new key
- Copy the public key  
<img src="img/CleanShot 2024-05-16 at 10.56.53@2x.png" alt="Copy key id" align="center" width="800"/>
- Paste the public key in Github settings  
<img src="img/CleanShot 2024-05-16 at 10.54.31@2x.png" alt="Copy key id" align="center" width="800"/>
- Copy key id  
<img src="img/CleanShot 2024-05-16 at 10.56.53@2x.png" alt="Copy key id" align="center" width="800"/>
- Run this `git config --global  user.signingkey <key id>`

