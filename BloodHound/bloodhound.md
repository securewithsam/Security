#### How To Install and Configure Neo4j on Ubuntu 20.04
```sh
sudo apt-get install openjdk-11-jdk
curl -fsSL https://debian.neo4j.com/neotechnology.gpg.key |sudo gpg --dearmor -o /usr/share/keyrings/neo4j.gpg
echo "deb [signed-by=/usr/share/keyrings/neo4j.gpg] https://debian.neo4j.com stable 4.1" | sudo tee -a /etc/apt/sources.list.d/neo4j.list
sudo apt update
sudo apt-get install apt-transport-https
sudo apt-get install neo4j
sudo systemctl stop neo4j
cd /usr/bin
sudo ./neo4j console
sudo systemctl start neo4j

sudo systemctl enable neo4j.service
sudo systemctl start neo4j.service
sudo systemctl status neo4j.service

```

#### Extract AD Data to import in BloodHound GUI
```sh
wget https://github.com/BloodHoundAD/BloodHound/releases/download/v4.3.1/BloodHound-linux-x64.zip
unzip BloodHound-linux-x64.zip
cd BloodHound-linux-x64
chmod +x BloodHound
apt install python3-pip
pip install bloodhound

apt install libgtk2.0-0 -y
sudo apt install libgtk-3-0 -y
nano /etc/resolv.conf
change the name server to the dc ip
bloodhound-python -u svc_test123 -p test123 -d sws.corp -dc FPP-INFDC-01.sws.corp


```
 
