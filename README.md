### How to deploy sonar Qube on your vagrant sonar 

Pre-requizite : 

SSH to your sonar server

```
vagrant ssh sonar-server

```
change this "sonar-server" to your vagrant sonar server name 

1. Change script permission 

```
chmod +x sonarQube_install.sh

```

2. Make sure Firewall opened for port 9000 & 22

```
sudo ufw enable
sudo ufw allow 9000
sudo ufw allow 22

```
3. Run the script

```
./sonarQube_install.sh

```

4. After self reboot access sonarQube on your Vagrant SonarIP:9000 on any browser