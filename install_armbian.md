# Installing and configuring Armbian

1.	Download [Armbian](https://www.armbian.com/orange-pi-zero-plus/#kernels-archive-all) and write to the microSD [Etcher](https://www.balena.io/etcher/)

2.	Сonnect via ssh (LAN):
```sh
ssh root@IP
```
password default:1234

3.	Add new user and reboot:
```sh
reboot
```

4.	Сonnect via ssh new user and Armbian configuring:
![main](img/1.png "1")
```sh
sudo apt-get update
sudo apt-get upgrade
reboot
```
```sh
sudo timedatectl set-timezone Europe/Moscow
```

5.	Connect to wi-fi:
```sh
sudo nmtui-connect
```
Edit a connection on static IP:
```sh
sudo nmtui
reboot
```
