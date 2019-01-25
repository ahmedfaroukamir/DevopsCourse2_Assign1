# nginx-container-reverse-proxy
if you want to create a reserve proxy for docker containers:

#
cd reverseProxy
#
docker build . -t reverseimage:1
#
docker run --name rc1 -d -p 9085:80 reverseimage:1
#
http://127.0.0.1:9085/
#
http://127.0.0.1:9085/bbc
#
http://127.0.0.1:9085/app1
#
http://127.0.0.1:9085/app2

#

<img width="790" alt="screen shot 2018-08-03 at 17 25 47" src="https://user-images.githubusercontent.com/20526165/43651626-2b8037d0-9743-11e8-9040-ffd1bd969f58.png">
