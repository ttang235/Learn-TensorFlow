# Using Tensorflow in docker
## Basic commands

```bash
docker run -it -p 8888:8888 gcr.io/tensorflow/tensorflow  # start to run the tensorflow image
docker ps  # show running docker instances
docker exec -it 204a03ccf44f /bin/bash  # run bash inside the running instance
apt-get update # update software source list
apt-get install -y wget # install wget (I need it for downloading), -y means 'yes', see https://askubuntu.com/questions/672892/what-does-y-mean-in-apt-get-y-install-command
```
