# Linux Guide
![alt text](https://pbs.twimg.com/profile_images/665149483827642368/Akvu1zUu.png "CyberPatriot")


&nbsp;

### Software:

Command Line Update:

* Google the correct contents for your sources file then place it in /etc/sources:

```bash
$ sudo gedit /etc/sources
$ sudo apt-get update
$ sudo apt-get upgrade
```

Search for installed program:
```bash
$ dpkg -l | grep <program name>
```

Uninstall program:
```bash
$ sudo apt-get remove --purge <program>
```
___

### User Accounts:
View user accounts:

```bash
$ sudo gedit /etc/shadow
$ sudo gedit /etc/passwd
```
___
### Services:

Start a service:

```bash
$ sudo service <service name> start
```

Stop a service:

```bash
$ sudo service <service name> stop
```
___
### Process/Network:
List all processes:
```bash
$ ps -fAH
```
Look for the following "bad" processes:
	
   * nmap
   * john
   * netcat/nc/ncat

Kill process:
```bash
$ pkill <process>
$ kill -9 <program PID>
```

List network connections:
```bash
$ netstat -naptu
```
### Stuff used to make this:
