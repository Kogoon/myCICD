install docker & ansible to amazon ami

~~~ bash
#!/bin/bash
timedatectl set-timezone Asia/Seoul
hostnamectl set-hostname ansible-server
amazon-linux-extras install -y ansible2
amazon-linux-extras install docker -y
systemctl enable --now docker
curl https://raw.githubusercontent.com/docker/docker-ce/master/components/cli/contrib/completion/bash/docker -o /etc/bash_completion.d/docker.sh
usermod -a -G docker ec2-user
~~~
