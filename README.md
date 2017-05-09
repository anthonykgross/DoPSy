# DoPSy : (DOcker, Php7 & SYmfony3)

## Requierements: 
- Docker 1.9
- Docker Compose 1.4

## Directory 
- docker    // Images docker & conf (Php7, nginx, supervisor & logs)
- docs      // Documentations
- src       // Symfony3 - Project source code

## How to install 

Create images for Docker
```console
chmod +x create-images.sh
./create-images.sh
```

Define permissions in folders & conf files
```console
chmod +x install.sh
./install.sh
```

Install vendor
```console
docker-compose run php7 install
```

Run the cluster (web + mysql + storage)
```console
docker-compose up
```

## Development 

- Don't miss to add 127.0.0.1 dopsy.local in /etc/hosts (Unix)
- Don't miss to add <VM ip> dopsy.local in /etc/hosts (OSX) or in Windows/System32/drivers/etc/hosts (Win)

## Creator

**Anthony K GROSS**
- <http://anthonykgross.fr>
- <https://twitter.com/anthonykgross>
- <https://github.com/anthonykgross>
- <http://www.twitch.tv/anthonykgross>

## Technologies
- PHP7 - Symfony 3 - Composer - PhpUnit
- LESS
- Bootstrap
- Bower
- Gulp
- MySql
