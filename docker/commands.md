
 - build image

`docker build -t webserver:latest -f docker/webserver/Dockerfile docker/webserver`

 - run container

`docker run --rm -d -p 8080:80 -v /$(pwd)/application:/var/www/html/public webserver`

 - docker copy from container to host

 ` docker cp goofy_roentgen:/out_read.jpg .`