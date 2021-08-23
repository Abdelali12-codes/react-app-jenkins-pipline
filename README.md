## Demo
https://youtu.be/OHyKaceFi8Q

## create reactjs app's jenkins pipline

## setup Jenkins on EC2

# install java
```
sudo apt-get update
sudo apt-get install -y openjdk-8-jdk
java -version
```

# install jenkins
```
wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > \
   /etc/apt/sources.list.d/jenkins.list'
sudo apt-get update
sudo apt-get install jenkins -y
sudo service jenkins start
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```

# install nodejs and npm
```
sudo apt-get install -y curl
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get install -y nodejs
```
# give the jenkins user the privilige of the root user (sudo.....)
```
echo "jenkins ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers
```
