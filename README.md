# DevopsCourse2_Assign1
Devops Course, 2nd session, 1st Assignment

# create docker containers


cd reverseProxy

docker build . -t reverseimage:1

docker run --name reversecontainer -d -p 9085:80 reverseimage:1


http://127.0.0.1:9085/bbc

cd ./app1

docker build . -t app1:1

docker run --name app1c -d -p 9081:80 app1:1

http://127.0.0.1:9085/app1

cd ./app2

docker build . -t app2:1

docker run --name app2c -d -p 9082:80 app2:1

http://127.0.0.1:9085/app2

# OR run docker compose

docker-compose up

#

<img width="790" alt="screen shot 2018-08-03 at 17 25 47" src="https://user-images.githubusercontent.com/20526165/43651626-2b8037d0-9743-11e8-9040-ffd1bd969f58.png">
