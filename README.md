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
### Add the repository to Apt sources:
~~~
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
~~~

### Install Dokcer Packages
~~~
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
~~~

## Quick installation Jump Server 

~~~
curl -sSL https://github.com/jumpserver/jumpserver/releases/latest/download/quick_start.sh | bash
~~~


