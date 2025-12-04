[ec2-user@ip-172-31-7-164 POC3]$ history
    1  clear
    2  ls -al
    3  clear
    4  sudo apt update
    5  sudo yum update
    6  sudo wget -O /etc/yum.repos.d/jenkins.repo \
    7  sudo wget -O /etc/yum.repos.d/jenkins.repo     https://pkg.jenkins.io/redhat-stable/jenkins.repo
    8  sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key
    9  sudo yum upgrade
   10  sudo yum upgrade -y
   11  sudo yum install fontconfig java-21-openjdk
   12  sudo yum install fontconfig java-17-openjdk
   13  sudo yum install java-17-openjdk -y
   14  sudo yum install java-17-amazon-corretto -y
   15  sudo yum install jenkins
   16  sudo systemctl daemon-reload
   17  systemctl status jenkins
   18  systemctl enable jenkins
   19  sudo systemctl enable jenkins
   20  systemctl status jenkins
   21  systemctl start jenkins
   22  sudo systemctl start jenkins
   23  systemctl status jenkins
   24  cat /var/lib/jenkins/secrets/initialAdminPassword
   25  sudo cat /var/lib/jenkins/secrets/initialAdminPassword
   26  git clone https://github.com/techcoms/springboot-app.git
   27  sudo yum install git -y
   28  git clone https://github.com/techcoms/springboot-app.git
   29  cd springboot-app/
   30  ls
   31  history
   32  cat Dockerfile 
   33  cat Jenkinsfile 
   34  cd ..
   35  ls
   36  git clone https://github.com/AnushaAkkena/POC3.git
   37  ls
   38  cd springboot-app/
   39  ls
   40  cp src Dockerfile /home/ec2-user/POC3
   41  cp -r src Dockerfile /home/ec2-user/POC3
   42  cd ..
   43  cd POC3/
   44  ls
   45  git status
   46  cd ../springboot-app/
   47  ls
   48  cp -r pom.xml /home/ec2-user/POC3
   49  cd ../POC3
   50  ls
   51  sudo yum install mvn
   52  sudo yum install maven
   53  mvn --version
   54  mvn clean package
   55  ls
   56  sudo amazon-linux-extras install docker -y
   57  sudo yum amazon-linux-extras install docker -y
   58  sudo yum install docker -y
   59  systemctl status docker
   60  systemctl enable docker
   61  sudo systemctl enable docker
   62  sudo systemctl start docker
   63  systemctl status docker
   64  ls
   65  docker build -t firstdocker .
   66  sudo chmod 777 /var/run/docker.sock
   67  docker build -t firstdocker .
   68  docker images
   69  docker run -d --name javaappliction-poc3 -p 80:80 firstdocker
   70  docker ps 
   71  docker inspect 72
   72  docker rm -r 72
   73  docker rm 72
   74  docker rm -f 72
   75  docker run -d --name javaappliction-poc3 -p 80:8080 firstdocker
   76  ls
   77  cd src
   78  ls
   79  cd main/
   80  ls
   81  cd java
   82  ls
   83  cd /abhishek/StartApplication.java
   84  cd /com
   85  cd com
   86  ls 
   87  cd abhishek/
   88  ls
   89  vi StartApplication.java 
   90  cd ../
   91  cd abhishek/
   92  pwd
   93  cp StartApplication.java /home/ec2-user/POC3/src/main/java/com/
   94  cd ..
   95  ls
   96  rm abhishek/
   97  sudo rm abhishek/
   98  rmdir abhishek/
   99  rmdir -r abhishek/
  100  rmdir -f abhishek/
  101  rm -rm abhishek/
  102  rm -rf abhishek/
  103  ls
  104  cd ..
  105  mvn clean package
  106  git status
  107  git add .
  108  git status
  109  git commit -m "commitning entire code"
  110  git status
  111  git push origin master
  112  git push https://github.com/AnushaAkkena/POC3.git
  113  git branch -M main
  114  git push -u origin main
  115  mvn clean package
  116  java --version
  117  history
  118  git pull https://github.com/AnushaAkkena/POC3.git
  119  cd POC3/
  120  git pull
  121  ls
  122  cd src
  123  ls
  124  cd main
  125  ls
  126  cd java/
  127  ls
  128  cd com
  129  ls
  130  git rm -f StartApplication.java 
  131  ls
  132  cd ../..
  133  mvn clean package
  134  systemctl status jenkins
  135  systemctl status docker
  136  docker ps
  137  sudo docker ps
  138  sudo docker ps -a
  139  sudo chmod 777 /var/run/docker.sock
  140  sudo docker ps
  141  sudo docker ps -a
  142  git push origin main
  143  git status
  144  git add .
  145  git commit -m "file deleted"
  146  git status
  147  git push origin main
  148  history
  149  sudo cat /var/lib/jenkins/secrets/initialAdminPassword
  150  docke ps -a
  151  docker ps -a
  152  docker rm d1
  153  git pull
  154  ls
  155  cd src/java/com
  156  cd src
  157  ls
  158  cd main/
  159  cd java/
  160  cd com
  161  ls
  162  cd ../..
  163  mvn clean package
  164  cd src/main/java/com
  165  ls
  166  rm -rf abhishek/
  167  ls
  168  cd ../../../
  169  cd ../
  170  mvn clean package
  171  git status
  172  git add .
  173  git status
  174  git commit -m "commited changes"
  175  git push origin main
  176  docker build -t firstproject:latest .
  177  history
  178  docker run -d --name javaappliction-poc3 -p 80:80 firstdocker
  179  docker ps
  180  docker rm a5
  181  dokecr -rm f a5
  182  docker -rm f a5
  183  docker ps
  184  docker rm a5
  185  docker ps -a
  186  sudo chmod 777 /var/run/docker.sock
  187  docker ps 
  188  docker rm a5
  189  docker rm -f a5
  190  docker run -d --name javaappliction-poc3 -p 80:8080 firstdocker
  191  docker images
  192  docker run -d --name javaappliction-poc3 -p 80:8080 firstproject
  193  docker run -d --name javaappliction-poc -p 80:8080 firstproject
  194  docker ps
  195  docker rm -f a9
  196  docker run -d --name javaappliction-poc -p 80:8080 firstproject
  197  docker run -d --name javaappliction-poc -p 80:8081 firstproject
  198  docker ps -a
  199  docker rm -f 02
  200  docker ps -a
  201  docker run -d --name javaappliction-poc -p 80:8081 firstproject
  202  docker ps
  203  docker rm -f ac
  204  docker ps
  205  docker run -d --name javaappliction-poc -p 81:8080 firstproject
  206  history

