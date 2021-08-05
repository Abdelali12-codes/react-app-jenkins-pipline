## create reactjs app's jenkins pipline

# setup Jenkins on EC2

- #!/bin/bash
- sudo yum update -y
- sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat/jenkins.repo
- sudo rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key
- sudo yum install java-1.8.0 -y
- sudo yum install jenkins -y
- sudo service jenkins start

- sudo cat /var/lib/jenkins/secrets/initialAdminPassword



sudo apt-get install curl
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get install -y nodejs