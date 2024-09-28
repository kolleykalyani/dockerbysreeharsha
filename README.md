# dockerbysreeharsha

### Explain about Docker architecture ?

* In the Docker architecture there are three important components. They are:

1.Docker client   : Which is responsible for running commands.

2.Docker Daemon   : Which is a background daemon running in the Docker host. When we install docker it will       
                    it will install both docker client and docker daemon but we can connect to the remote host 
                    using docker client.
                    
3.Docker registry : Where we are going to push our images.

* First we need to update the sever

```
apt update
```

* Then need to install the requried tools

```
apt install -y net-tools jq unzip
```

* To install docker

```
curl https://get.docker.com | bash

```

* To see the docker running 

```
ps -ef | grep docker 
```

* To list the namesapces

```
lsns
```

* To list only pid namespaces or specific namespaces

```
 lsns -t pid 
```

* To split the putty screen

```
tmux 
```
(then press ctrl+b and shift double codes)
(to enter into upper screen ctrl+b & up arrow)
(to enter into lower screen ctrl+b & down arrow)

* To exit the tmux mode type

```
exit
```

* To create a conatiner with automatic remove option if container is exited

```
docker run --rm -d --name app1 -p 8000:80 nginx
```

* To craete multiple containers at a single time

```
for I in {1..5}
do
docker run --rm -d --name app$I -p 800$I:80 nginx
done
```

* To stop the all containers at a time

```
 docker stop `docker ps -aq`
```

* To list all  the running containers

```
docker ps -aq
```

* To list how many n/w are installed while installing docker

```
docker network ls
```

* To see the disk usage

```
df -h
```

* To delete docker images

```
docker rmi `docker images -aq` --force
```

* it shows how many volumes we have attached to the ec2 instances

```
lsblk
```
 
* To create the filesystem for the volume

```
 mkfs.ext4 /dev/xvdf
```

* To mount the volumes to the created directory

```
 mount /dev/xvdf /myvolume
```

* To add the filesystem uuid to the fstab

```
vi /etc/fstab
```

* To reload the daemon

```
 systemctl daemon-reload
```
