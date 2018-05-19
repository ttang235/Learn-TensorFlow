# Using Tensorflow in docker
## Basic setup commands

```bash
docker run -it -p 8888:8888 gcr.io/tensorflow/tensorflow  # start to run the tensorflow image
docker ps  # show running docker instances
docker exec -it 204a03ccf44f /bin/bash  # run bash inside the running instance
apt-get update # update software source list
apt-get install -y wget # install wget (I need it for downloading), -y means 'yes', see https://askubuntu.com/questions/672892/what-does-y-mean-in-apt-get-y-install-command
apt-get install vim
apt-get install git-core
```

To get a better experience using vim in docker, you may want a .vimrc file. If you run `echo $HOME`, you will get `/root`. So you can put your .vimrc there.

You can also put [this .inputrc](https://github.com/ttang235/BasicTerminalSetup/blob/master/.inputrc) file under `/root` to have a better history command search experience (type prefix and use up arrow to do prefix matching search). You need to `exit` and rerun the bash to let it take effect.
