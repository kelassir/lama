# Day 1

## Hands-On Part 1 
### Morning Session

- Download VMWare player and install
- Download Kali-vmware image and unzip
- Open Kali from VMWare and run
username = kali
password = kali
- Run Root Terminal Emulator in Kali
- Learning Commands
```
# passwd root
```
- Switch User / Logout
username = root
password = toor
- Open firefox
	- download jmeter
	- download jmeter-plugin-manager.jar
- Learning Commands
```
# sh
# clear
# ls
# tree
# tree -L 2
# cd
# cd /
# pwd
# java --version
# apt install openjdk-21-jre
# unzip apache-jmeter-5.6.3.zip
```

### Afternoon Session
```
# sh apache-jmeter-5.6.3/bin/jmeter.sh
# mv
```
Terminal > File > New Tab
```
# apt update
# apt upgrade
# apt install docker.io
# docker ps
# docker images
# tmux new -s docker
# w
```
CTRL+b lepas c
CTRL+b lepas c
ls
CTRL+b 1
CTRL+b 2
CTRL+b d
```
# tmux a -t docker
```
CTRL+b %
CTRL+b <--
CTRL+b "
CTRL+b d
```
# tmux new -s baru
# docker images
# docker pull wordpress
# docker images
```
CTRL+b d
```
# tmux ls

# tmux a -t baru
# exit

# tmux ls
```
firefox go to
hub.docker.com
search wordpress
scroll jumpa script
copy
open folder
create new folder
lama
open lama
create new empty file
docker-compose.yml
paste dalam file tadi


open new terminal
```
# ls
# cd lama

# tmux new -s lama
# ls
```
CTRL+b c
```
# while true
> do
> clear
> docker ps -a
> sleep 5
> done
```
CTRL+b "
```
#docker-compose up
```
install wp

CTRL+b %
```
# while true
> do
> clear
> docker images
> sleep 5
> done
```
CTRL+b ke atas
CTRL+b "
```
# docker pull grafana/k6
```
copy script dari github.com/kelassir/lama
CTRL+b c
```
# mkdir kelassir
# touch kelassir/docker-compose.yml
```
_masuk ke folder kelassir_
```
# cd kelassir
```
open folder kelassir
open docker-compose.yml
paste
```
# pwd
```
make sure /root/lama/kelassir

_nak up docker container_
```
# docker-compose up
```

# Day 2
## Hands-On Part2 
## Troubleshooting
```
# docker ps
# docker stop namakontainer1 namakontainer2

# docker ps -a
# docker rm namakontainer1 namakontainer2

# docker images
# docker image rm namaimage1 namaimage2

# docker network list
# docker network rm namanetwork1 namanetwork2

# docker system prune

# docker volume list
# docker volume rm namavolume1 namavolume2
```
### Morning Session
```
# docker run --rm -p 44444:80 -e PMA_ARBITRARY=1 phpmyadmin/phpmyadmin

# docker pull drupal
# docker run -p 60000:80 --name drupal2 drupal
```

### Afternoon Session
ask chatgpt "berikan saya script k6 untuk load testing 1, 10, 100 http://ipaddress:60000/en"

keluar dari tmux lama
CTRL+b d
```
# cd
```
buat tmux baru
```
# mkdir k6
# touch k6/11-load.js
# touch k6/12-load.js
```
paste script dari chatgpt ke touched files
```
# cd k6
# tmux new -s k6
```
CTRL+b c
```
# docker run --rm -i grafana/k6 run - < 11-load.js
```
