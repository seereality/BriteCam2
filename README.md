# BriteCam2
BriteCam2 is WebRTC based video recording web app built on Tornado and Kurento Media Server.

Kurento Media Server has to be installed on Ubuntu 14.04 LTS (32 or 64 bits).
##Intruction to Install KMS
```
  sudo apt-get install software-properties-common # To install add-apt-repository tool
  sudo add-apt-repository ppa:kurento/kurento
  sudo apt-get update
  sudo apt-get install kurento-server

```
Now, Kurento Media Server has been installed and started. Use the following commands to start and stop it respectively:

```
sudo service kurento-media-server start
sudo service kurento-media-server stop

```

Kurento Media Server has a log file located at `/var/log/kurento-media-server/media-server.log`.

After Installing KMS.

## Developing

### Source and deps

```
git clone https://github.com/seereality/BriteCam2
cd ./BriteCam2
pip install -r requirements.txt
```

### Running the example

```
./app.py
```

There are a couple of assumptions the example makes.
* You want to run on port 8080 - its hardcoded in there at the moment
* Your KMS address is localhost:8888 - again, hardcoded

