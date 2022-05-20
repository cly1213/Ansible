# Tomcat installation on EC2 instance

### Prerequisites
1. EC2 instance

### Install Apache Tomcat
Install Java 
```sh
   yum install java
```

Download tomcat packages from https://tomcat.apache.org/download-90.cgi onto /opt on EC2 instance
```sh
  # create tomcat directory
  cd /opt
  wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.63/bin/apache-tomcat-9.0.63.tar.gz
  tar -xvzf /opt/apache-tomcat-9.0.63.tar.gz
```
give executing permissions to startup.sh and shutdown.sh which are under bin.
```sh
   chmod +x /opt/apache-tomcat-9.0.63/bin/startup.sh shutdown.sh
```
start the tomcat services
```
  cd /opt/apache-tomcat-9.0.63/bin
  ./startup.sh

```
#### check point :
access tomcat application from browser on prot 8080
http://<Public_IP>:8080


