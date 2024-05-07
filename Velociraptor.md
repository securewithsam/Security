#### Velociraptor 

```sh


       apt update
       apt upgrade -y
       mkdir velociraptor
       cd velociraptor/
       https://github.com/Velocidex/velociraptor/releases/download/v0.72/velociraptor-v0.72.0-linux-amd64
       wget https://github.com/Velocidex/velociraptor/releases/download/v0.72/velociraptor-v0.72.0-linux-amd64
       cp velociraptor-v0.72.0-linux-amd64 /usr/local/bin/velociraptor
       chmod +x /usr/local/bin/velociraptor
       velociraptor config generate -i
       nano /etc/velociraptor.config.yaml
       nano /lib/systemd/system/velociraptor.service
       systemctl daemon-reload
       systemctl enable --now velociraptor
       systemctl status velociraptor
       ss -antpl | grep 8889
       history



```
