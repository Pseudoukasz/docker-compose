**Cel: Stworzenie serwera z usługą LAMP

Potrzebne pliki:
-ApacheDocker
    -apache.conf
    -Dockerfile
-PHPDocker
    -php.ini
    -Dockerfile
-MySQL
    -my.cnf
    -Dockerfile
-files
    -index.html
    -index.php
-docker-compose.yml

*Wykonianie:

tworzenie projektu poleceniem:
```
docker-compose build
```
uruchomienie projektu poleceniem: 
```
docker-compose up
```
podgląd działania systemu:
```
curl localhost:6666/ 
```
podgląd html:

polecenie:
```
curl localhot:6666/index.html
 ```
Wizualiacja stowrzonego servera:
 ```
ocker run --rm -it --name dcv -v $(pwd):/input pmsipilot/docker-compose-viz render -m image docker-compose.yml
 ```
