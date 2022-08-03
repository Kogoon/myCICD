In Jenkins

Configure  

`Send files or execute commands over SSH` -> `Exec command`

~~~ 
cd /opt/docker;
ansible-playbook build.yaml;
sleep 10;
ansible-playbook deploy.yaml
~~~


