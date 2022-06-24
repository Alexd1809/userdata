#!/bin/bash
cat << EOF > userdata.sh
#!/bin/bash
sudo apt update -y
scp ssh-copy-id 82.64.98.187:2222
sudo apt install MariaDB-server -y
sudo systemctl enable --now mariadb
sudo mariadb-secure-installation <<EOF

y
password
password
y
y
y
y
EOF
