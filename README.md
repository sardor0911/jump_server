# jump_server
Jump Server fit2cloud

# Installation PAM (Privileged Access Management) System Jump Server 
## Install unitilies for Jump Server

~~~
apt-get install -y wget curl tar gettext iptables
~~~
## Install Docker 
### Install using the apt repository
~~~sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc
sudo apt-get update
~~~
## Quick installation Jump Server 

~~~
curl -sSL https://github.com/jumpserver/jumpserver/releases/latest/download/quick_start.sh | bash
~~~


