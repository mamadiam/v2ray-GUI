## Use the following commands on your IR Server</br>

#### 1. Update & upgrade the packages </br>
```shell script
sudo apt update && apt upgrade -y
``` 
#### 2. Run the following commands all at once </br>
First change the `YOUR_IR_SERVER_IP` & `YOUR_NON_IR_SERVER_IP`</br>
```shell script
sysctl net.ipv4.ip_forward=1
iptables -t nat -A PREROUTING -p tcp --dport 22 -j DNAT --to-destination YOUR_IR_SERVER_IP
iptables -t nat -A PREROUTING -j DNAT --to-destination YOUR_NON_IR_SERVER_IP
iptables -t nat -A POSTROUTING -j MASQUERADE
``` 
Only use the following command if you have slow connections and got disconnected repeatedly </br>
#### 3. If you have slow connections </br>
```shell script
wget -N --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh && chmod +x bbr.sh && bash bbr.sh
```
