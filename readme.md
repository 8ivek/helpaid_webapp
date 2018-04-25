## Running the app

### Docker build
$ docker build -t bivek/helpaid_webapp .

### Docker run
$ docker run -p 49160:8080 -d bivek/helpaid_webapp

### Enter inside the container
$ docker exec -it <container id> /bin/bash
> not working for me

### List running containers
$ docker ps

__Example__

ID  IMAGE  COMMAND    ...   PORTS

ecce33b30ebf  bivek/node-web-app:latest  npm start  ...  49160->8080

### Running program
$ curl -i localhost:49160

Output: 

HTTP/1.1 200 OK
X-Powered-By: Express
Content-Type: text/html; charset=utf-8
Content-Length: 12
ETag: W/"c-M6tWOb/Y57lesdjQuHeB1P/qTV0"
Date: Mon, 13 Nov 2017 20:53:59 GMT
Connection: keep-alive

Hello world

