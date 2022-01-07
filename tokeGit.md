ozeias@barreto:~$ ssh-keygen -t ed25519 -C ozbarreto@outlook.com
Generating public/private ed25519 key pair.
Enter file in which to save the key (/home/ozeias/.ssh/id_ed25519): 
/home/ozeias/.ssh/id_ed25519 already exists.
Overwrite (y/n)? y
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/ozeias/.ssh/id_ed25519
Your public key has been saved in /home/ozeias/.ssh/id_ed25519.pub
The key fingerprint is:
SHA256:Hu/qakAy7XSU6iOOvvx0VYfrKIzGHL9bnq8/CCwFHbA ozbarreto@outlook.com
The key's randomart image is:
+--[ED25519 256]--+
|   .o...         |
|   ...o   .      |
|   E.o   o .     |
|  o =.. . o      |
|   Oo. .S.       |
|  +.Xo..oo       |
| o B.B.oo..      |
|o + . *..o       |
|.+o. +o**+o      |
+----[SHA256]-----+
ozeias@barreto:~$ cd .ssh/
ozeias@barreto:~/.ssh$ ls
id_ed25519  id_ed25519.pub  known_hosts
ozeias@barreto:~/.ssh$ cat id_ed25519.pub 
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIKhvJuQIm5+Y6ugO/qD3G01OynFGYU6j6kv1mso/OWTt ozbarreto@outlook.com
ozeias@barreto:~/.ssh$ eval $(ssh-agent -s)
Agent pid 7508
ozeias@barreto:~/.ssh$ ssh-add id_ed25519
Enter passphrase for id_ed25519: 
Identity added: id_ed25519 (ozbarreto@outlook.com)
ozeias@barreto:~/.ssh$
