```bash
sudo nano /etc/security/group.conf
```

```
*;*;*;Al0000-2400;dialout 
```
 
```bash
sudo nano /etc/pam.d/common-auth
```

```
auth	required			pam_group.so 
```
 
```
sudo pam-auth-update 
```
 
```
reboot
```