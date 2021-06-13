Fallowing are steps forl ogin service in Todoapp.

#apt update

#useradd -m -s /bin/bash app

#cd /home/app

#wget -c https://dl.google.com/go/go1.14.2.linux-amd64.tar.gz -O - | sudo tar -xz -C /usr/local

#export PATH=$PATH:/usr/local/go/bin

#source ~/.profile

#go version

#mkdir ~/go

#mkdir -p ~/go/src

#cd  ~/go/src/

#git clone https://github.com/zelar-soft-todoapp/login.git

#cd login/

#apt update

#apt install go-dep

#go get

#go build

#vim /etc/systemd/system/login.service

#systemctl daemon-reload

#systemctl start login.service

#systemctl enable login.service
   
#systemctl status login.service
   
   -----------------systemd files === login.service files-------------------
   
[Unit]
Description = login Service

[Service]
user=root
Environment=AUTH_API_PORT=8080
Environment=USERS_API_ADDRESS=http://172.31.90.28:8080
ExecStart=/root/go/src/login/login
SyslogIdentifier=login

[Install]
WantedBy=multi-user.target
