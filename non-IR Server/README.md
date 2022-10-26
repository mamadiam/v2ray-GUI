## Use the following commands on your non-IR Server</br>

#### 1. Update & Upgrade the packages </br>
```shell script
sudo apt update && apt upgrade -y
``` 
#### 2. Install curl on your server </br>
```shell script
sudo apt install curl -y
```
#### 3. Run this command </br>
```shell script
bash <(curl -Ls https://raw.githubusercontent.com/vaxilu/x-ui/master/install.sh)
```
#### 4. Login to admin panel </br>
```shell script
YOUR_SERVER_IP_ADDRESS:54321
```
You Can login to your Panel with the following credentials. </br>
Username `admin` Password `admin`</br></br>
The app is in chinese, so use google chrome as your web browser, right click on the page and choose `translate to English`</br>
After you loged in into your server natigate to `panel setting, user setting` and change your admin user `password`</br></br></br>
Only use the following command if you have slow connections and got disconnected repeatedly </br>
#### 5. If you have slow connections </br>
```shell script
wget -N --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh && chmod +x bbr.sh && bash bbr.sh
```
