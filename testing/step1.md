First if you run `whoami`{{execute HOST1}}, you will see that you are running as `root`. 

Users are also allowed to install tools to the scenario instance. As an example the user can install
nmap with `apt-get install nmap -y`{{execute HOST1}}

By design Katacoda scenarios allow the user to install containers to the running instance. 
As an example a user could install the docker version of Kali with the following commands: 

* `docker pull kalilinux/kali-rolling`{{execute HOST1}}

* `docker run -t -i kalilinux/kali-rolling /bin/bash`{{execute HOST1}}

* `apt-get update && apt-get upgrade -y`{{execute HOST1}}

As you can see katacoda allows for a great deal of flexibility. 

