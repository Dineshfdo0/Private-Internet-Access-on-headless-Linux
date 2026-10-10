# Private-Internet-Access-on-headless-Linux

echo "nameserver 1.1.1.1" | sudo tee /etc/resolv.conf

wget https://installers.privateinternetaccess.com/download/pia-linux-3.5.7-08120.run -O pia-installer.run

./pia-installer.run

nano ~/pia-login.txt

->>>>>>>>>>>> pia-login.txt -- contaent ->>>>>>>>>>>>"
***my pia user*** 
***my pia pass***
->>>>>>>>>>>> pia-login.txt -- contaent ->>>>>>>>>>>>"

piactl login ~/pia-login.txt

 piactl connect

piactl get connectionstate

curl https://ifconfig.me

piactl set region switzerland



Action	Command
Check Connection Status	---> piactl get connectionstate
Disconnect VPN	---> piactl disconnect
Reconnect VPN	---> piactl connect
Check Current Public IP	---> piactl get vpnip
Enable Killswitch	---> piactl set killswitch auto



