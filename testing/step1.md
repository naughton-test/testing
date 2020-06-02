By design Katacoda scenarios allow the user to install containers to the running instance. 
As an example a user could install the docker version of Kali with the following commands: 

* `docker pull kalilinux/kali-rolling`{{execute HOST1}}
* `docker run -t -i kalilinux/kali-rolling /bin/bash`{{execute HOST1}}
* `apt-get update`{{execute HOST1}}

If you run `whoami`{{execute HOST1}}, you will also see that you are running as `root`. 