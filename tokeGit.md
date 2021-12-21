ssh-keygen -t ed25519 -C ozbarreto@outlook.com

eval $(ssh-agent -s)

```tex
ozeias@barreto:~$ cd .ssh/
ozeias@barreto:~/.ssh$ ls
id_ed25519  id_ed25519.pub  known_hosts
ozeias@barreto:~/.ssh$ cat id_ed25519
-----BEGIN OPENSSH PRIVATE KEY-----
b3BlbnNzaC1rZXktdjEAAAAACmFlczI1Ni1jdHIAAAAGYmNyeXB0AAAAGAAAABCLlj9rBs
JCgIbXgvDkhYIBAAAAEAAAAAEAAAAzAAAAC3NzaC1lZDI1NTE5AAAAIDYNm9iuMQLHssQ0
mCQLYGLSHLQ6+Pdfbox85QbgYxogAAAAoG+K2fKNcB8KSLeElReTDSjsJ/C+K5XPe/ACLU
+gMZDv4/6E/r7mQN8ul40DG6juSYgqgJqtEASlcrl5FzNXP3L8Yp5nIHWM8XCLFgqsXb1c
zRl9yA28IO+s/HLMu85qStW7s4VXuCTPk1qUv0xrVbqUJ2yNzomjzpfexxQ3wZDjD60/+z
hKyVrHr7vHKNwn2/o7hR4lsNTFU9NGDy0FCAk=
-----END OPENSSH PRIVATE KEY-----
ozeias@barreto:~/.ssh$ cat id_ed25519.pub 
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIDYNm9iuMQLHssQ0mCQLYGLSHLQ6+Pdfbox85QbgYxog ozbarreto@outlook.com
ozeias@barreto:~/.ssh$ ^C
ozeias@barreto:~/.ssh$ pwd
/home/ozeias/.ssh
ozeias@barreto:~/.ssh$ eval $(ssh-agent)
Agent pid 8044
ozeias@barreto:~/.ssh$ ^C
ozeias@barreto:~/.ssh$ ssh-add ^C
ozeias@barreto:~/.ssh$ ssh-add id_ed25519
Enter passphrase for id_ed25519: 
Identity added: id_ed25519 (ozbarreto@outlook.com)
ozeias@barreto:~/.ssh$ 

```

