# My Laravel Dockerized Project

This is a Laravel 10 project running on Docker, with MySQL and Nginx.

## 🚀 Requirements
- Ubuntu Server (tested on 22.04)
- Docker
- Docker Compose
- Git

## 🛠️ Setup Instructions

1. **Clone this repo**
```bash
sudo apt install git
git clone https://github.com/coldzamzam/laraveldocker.git
cd laraveldocker
```

2. ***Update & Upgrade***
```bash
sudo apt-get update && sudo apt-get upgrade
```

3. ***Install Docker & Docker Compose from Official Website***
```
# Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update

#Install the Docker packages
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

4. ***Build & Start Containers***
```
sudo docker compose build
sudo docker compose up -d
```

5. ***Open Localhost on Your Browser***
```
http://localhost:8000
```
OR
```
http://[yourIP]:8000
```



