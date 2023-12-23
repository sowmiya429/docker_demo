# docker_demo
Create Ec2 Instance 
![image](https://github.com/sowmiya429/docker_demo/assets/80743760/29c36e1e-473f-4501-ab8f-5a8445f719ca)
#update the system
```
sudo apt install -y
```
![image](https://github.com/sowmiya429/docker_demo/assets/80743760/6984f9f2-9d25-4b6a-8fb6-ab82c652b225)
Install Docker
```
sudo apt install docker.io -y
```
To check the status of the docker
```
sudo apt status docker
```
![image](https://github.com/sowmiya429/docker_demo/assets/80743760/595b0051-468e-4691-9385-c8b36e98988c)
To check the docker installed or not
```
docker run hello-world
```
First it will tell you permission denied
![image](https://github.com/sowmiya429/docker_demo/assets/80743760/8b8819ff-a28f-4ba8-9a9e-14981bf30c96)
-Why because initially docker installed on the root user it doesn't give permission to the root user
-To give permission to the UBUNTU user. Because here we use UBUNTU 
-Use the below command to give permission to the UBUNTU user
```
sudo usermod -aG docker ubuntu
```
-usermod --> modifying the user
-aG docker--> adding the ubuntu user to the docker group
After this still we got the same error
![image](https://github.com/sowmiya429/docker_demo/assets/80743760/9ebbbbd0-08bd-4ab0-a951-42d0fe167ed0)
Now, needs to logout and login the system again
![Uploading image.png…]()


