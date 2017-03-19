## Data Science Tool

### はじめに
本ツールは、Python3(Anaconda)とPostgreSQL9.5.3を利用して、データ解析、機械学習をするためのツールです。
docker-composeを使い、Ubuntuサーバを立ち上げ、そのなかでPython3で作業を行うことができます。
データベースと接続し、データを保存したりすることができます。

### 使い方
```
$ cd ~
$ git clone https://github.com/tomohitoy/datsci.git
$ mkdir ~/.ssh
$ cd .ssh
$ ssh-keygen -t rsa -b 4096 -C "t07840ty@gmail.com"
$ cp id_rsa.pub ~/datasci/
$ cd ~/datasci
$ docker-compose build
$ docker-compose pull
$ docker-compose up -d
$ ssh tomohitoy@0.0.0.0 -p 2222 -i ~/.ssh/id_rsa
```

