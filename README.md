## Simple DevOps Project -3 


1. Launch an EC2 instance for Jenkins and Docker 

2. Install jenkins & docker on EC2 instance and start services 
  ```
   Jenkins:
     sudo yum update
     sudo wget -O /etc/yum.repos.d/jenkins.repo \
     sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
     sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key
     sudo yum upgrade
     sudo yum upgrade -y
     sudo yum install fontconfig java-21-openjdk
     sudo yum install fontconfig java-17-openjdk
     sudo yum install java-17-openjdk -y
     sudo yum install java-17-amazon-corretto -y
     sudo yum install jenkins
     sudo systemctl daemon-reload
     systemctl status jenkins
     sudo systemctl enable jenkins
     systemctl status jenkins
     sudo systemctl start jenkins
     systemctl status jenkins
     
   Docker:
     sudo yum install docker -y
     systemctl status docker
     systemctl enable docker
     sudo systemctl enable docker
     sudo systemctl start docker
     systemctl status docker
  ```

4. Write a Docker file 

```
# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM adoptopenjdk/openjdk11:alpine-jre

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
```

5. Login to Jenkins console and add Docker server to execute commands from Jenkins  
Manage Jenkins --> Configure system -->  Publish over SSH --> add Docker server and credentials
installed jenkins pulgins manage jenkins > manage plugins > git, maven, docker

6. Create Jenkins job 

A) Source Code Management    
 Repository : https://github.com/AnushaAkkena/POC3.git   
 Branches to build : */main  

B) Build
 Root POM: pom.xml  
 Goals and options : clean install package  
   

7. Login to Docker instance and check images and containers. (no images and containers)

8. Execute Jenkins job

9. check images and containers again on Docker instance console. This time an image and container get creates through Jenkins job

10. Access web application from browser which is running on container
```
<docker_host_Public_IP>:80
```
