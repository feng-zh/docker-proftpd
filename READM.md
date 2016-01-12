Introduction
-----
This is the docker project to setup proftpd (FTP Server) with ldap supporting.


Install
-----
### Simple Run
```
docker run --name proftpd -p 20:20 -p 21:21 fengzhou/proftpd
```

### Customize Configuration File
```
# suppose configuration file is located in current folder.
docker run --name proftpd -p 20:20 -p 21:21 -v $(pwd)/proftpd.conf:/etc/proftpd.conf fengzhou/proftpd
```

The proftpd server configuration can refer to http://www.proftpd.org/docs/example-conf.html


Note
-----
This docker may enhance a bit later with supporting environment variable without explict external mounted configuration file. Stay tuned.

