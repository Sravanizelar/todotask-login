Fallowing are steps forl ogin service in Todoapp.

#apt update

#mkdir go

#cd go/

#mkdir src

#cd src/

#curl -O https://stroage.googleapis.com/golang/go1.13.5.linux-amd64.tar.gz

#tar -xvf go1.13.5.linux-amd64.tar.gz

#sudo mv go /usr/local

#export GOPATH=$HOME/WORK

#export PATH=$PATH:/usr/local/go/bin:$GOPATH/bin

#source ~/.profile

#go version

git clone https://github.com/zelar-soft-todoapp/login.git

#cd login/

#vi /etc/systemd/system/login.service

#go build

#go get github.com/dgrijalva/jwt-go

#go get github.com/labstack/echo

#go get github.com/labstack/echo/middleware

#go get github.com/labstack/gommon/log

#go get github.com/openzipkin/zipkin-go

#go get github.com/openzipkin/zipkin-go/middleware/http

#go get github.com/openzipkin/zipkin-go/reporter/http

#go build main.go user.go tracing.go

#go build

#systemctl daemon-reload

#systemctl start login

#systemctl enable login

#systemctl status login

