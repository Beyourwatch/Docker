# Docker

![image](https://user-images.githubusercontent.com/63569149/170415670-46f78cd9-b611-4535-b436-9b2353e9da75.png)

![image](https://user-images.githubusercontent.com/63569149/170415740-2ade2dac-2c5a-4720-9441-97996965e6aa.png)


docker image ls
docker container ps
docker image pull

docker run -it [image] bash // -i 交互 -t 赋予tty
--rm  退出后自动删除container

docker run -d -p 80:80 nginx  //-p 附加断开  -d 在后台 

docker exec -it container bash  //进入现场运行中的容器

删除
docker rm containerID
docker rmi imageID

导出
docker save hello-world:latest > myhelloworld.tgz
导入
docker image load -i /home/bb6/Desktop/myhelloworld.tgz
