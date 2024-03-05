SSH setup:
Generate public key 

ssh-keygen -t rsa

Copy the public key to Grafana server 

ssh-copy-id <grafana_username>@<grafana_server_ip>

Now ssh to grafana:

ssh <grafana_username>@<grafana_server_ip>


Static Inventory file:

/etc/<server:_name>/hosts


[grafana server]
ip_address ansible_name=username ansible_password=password
