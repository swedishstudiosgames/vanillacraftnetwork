## Create an Docker volume

`docker volume create minecraft-crossplay-server`


## Create an Docker image

`docker run -it -v minecraft-crossplay-server:/minecraft -p 25565:25565 -p 19132:19132/udp -p 19132:19132 -e MaxMemory=4096 -e TZ="Europe/Stockholm" --restart unless-stopped 05jchambers/legendary-minecraft-geyser-floodgate:latest`


## Check the Docker volume

`docker volume inspect minecraft-crossplay-server`
