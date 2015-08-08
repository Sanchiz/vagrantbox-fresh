Credentials
===
IP - 192.168.77.77

User - root

Password - root

How to use
===

```sh
vagrant up
ssh-copy-id root@192.168.77.77
```

If you see message

```
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@    WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED!     @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
IT IS POSSIBLE THAT SOMEONE IS DOING SOMETHING NASTY!
Someone could be eavesdropping on you right now (man-in-the-middle attack)!
It is also possible that a host key has just been changed.
The fingerprint for the RSA key sent by the remote host is
db:30:e8:c5:08:ce:4c:bf:a3:06:bd:f7:bb:7e:19:68.
Please contact your system administrator.
Add correct host key in /Users/sanchiz/.ssh/known_hosts to get rid of this message.
Offending RSA key in /Users/sanchiz/.ssh/known_hosts:70
RSA host key for 192.168.77.77 has changed and you have requested strict checking.
Host key verification failed.
```

Use following commands:
```sh
ssh-keygen -R 192.168.77.77
ssh-copy-id root@192.168.77.77
# enter "root" as password
```


Then you will be able to use Ansible!
