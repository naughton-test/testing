First if you run `whoami`{{execute HOST1}}, you will see that you are running as `root`. 

The scenario is build with a specific goal in mind, however users are able to install tools onto the instance. 
As an example if you install net-tools `apt install net-tools`{{execute HOST1}} into the scenario this will allow you to get the hosts IP
by using `ifconfig`{{execute HOST1}}. Please make a copy of this address as it will be used later. 172.17.0.53

By design Katacoda scenarios allow the user to install containers to the running instance. 
As an example a user could install the docker version of Kali with the following commands: 

* `docker pull kalilinux/kali-rolling`{{execute HOST1}}

* `docker run -t -i kalilinux/kali-rolling /bin/bash`{{execute HOST1}}

* `apt-get update && apt-get upgrade -y`{{execute HOST1}}

Within the kali instacne you can install nmap with `apt-get install nmap -y`{{execute HOST1}}

Once nmap has been installed attempt to run a ping sweep

`nmap -sP xxx.xxx.1-255.1-255` where the x's are the first two octets of the address. 

```Starting Nmap 7.80 ( https://nmap.org ) at 2020-06-03 14:47 UTC
Connection to docker closed by remote host.
Connection to docker closed.

The environment has expired.

Please refresh to get a new environment.```

Katacoda scenarios are hardened to not allow this, and other activites. 
