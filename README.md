# VICIDIAL INSTALLATION SCRIPTS
# Centos7 Vicidial Install pre_requisites 

```
### Use YOUR SubDomain
hostnamectl set-hostname xxxxxx.xxxxx.xxx

vi /etc/hosts
##Change domain name for actual server ip (xxx.xxx.xxx.xxx   complete domain name    subdomain only)

timedatectl set-timezone America/New_York

yum check-update
yum update -y
yum -y install epel-release
yum update -y
yum install git -y
yum install -y kernel*

#Disable SELINUX
sed -i 's/SELINUX=enforcing/SELINUX=disabled/g' /etc/selinux/config    

reboot

````
  Reboot Before running this script

# Install VICIDIAL scripts

```
git clone https://github.com/GenXoutsourcing/vicidial-install-scripts.git
cd vicidial-install-scripts
```

# Execute Centos7 Vicidial Install
```
chmod +x vicidial-install-c7.sh
./vicidial-install-c7.sh
```

# Excute Ubuntu Vicidial Install (coming soon)
```
chmod +x vicidial-install-ubuntu18.sh
./vicidial-install-ubuntu18.sh
```

# Install WEBRTC for VICIDIAL Now (coming soon)
# DO THIS IF YOU HAVE PUBLIC DOMAIN WITH PUBLIC IP ONLY

```
chmod +x vicidial-enable-webrtc.sh
./vicidial-enable-webrtc.sh
```
