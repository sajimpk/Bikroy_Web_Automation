# Docker Run Via Jenkin

## Install Java:
```
sudo apt update
```
```
sudo apt install openjdk-17-jdk
```

## Install Jenkin:

```
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
```
```
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
```
```
sudo apt-get update
```
```
sudo apt-get install jenkins
```

## Docker Install:

```
sudo apt-get update
```
```
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common
```
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```
```
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```
```
sudo apt-get update
```
```
sudo apt-get install docker-ce
```
```
sudo docker run hello-world
```

### Set Custom Port 8080 on AWS iN security group.

### Give Permission: For Docker Run Via Jenkin
```
sudo usermod -aG docker jenkins
```
```
sudo systemctl restart jenkins
```


## Docker Run:

```
sudo docker build -t Bikroy_Web_Automation .
```
```
sudo docker run --rm Bikroy_Web_Automation
```
