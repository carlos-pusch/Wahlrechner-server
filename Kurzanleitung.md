# Kurzanleitung

```
sudo mkdir /opt/wahlrechner-server/
sudo git clone --recurse-submodules https://github.com/carlos-pusch/Wahlrechner-server /opt/wahlrechner-server/

cd /opt/wahlrechner-server

docker rm $(docker ps -aq) --force
```

In /opt

```
sudo chmod -R u+rwx wahlrechner-server
sudo chown -R carlos:carlos wahlrechner-server
```

anpassen von global.env | 3 PWDs

falls vergessen /opt/wahlrechner-server löschen und neustarten

```
sudo systemctl restart docker
sudo bash ServerUpdate.sh
```
