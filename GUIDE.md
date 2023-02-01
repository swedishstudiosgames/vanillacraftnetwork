## Create an Docker volume

`docker volume create yourvolumenamehere`


## Create an Docker image

`docker run -it -v yourvolumenamehere:/minecraft -p 25565:25565 -p 19132:19132/udp -p 19132:19132 -e MaxMemory=yourmaxrammemoryhere -e TZ="yourtimezonehere" --restart unless-stopped 05jchambers/legendary-minecraft-geyser-floodgate:latest`


## Check the Docker volume

`docker volume inspect yourvolumenamehere`
