1. docker run -p 9200:9200 --name elasticsearch -e "discovery.type=single-node" elasticsearch:7.5.1


docker network create elk

docker run -p 9200:9200 --network elk --name elasticsearch -e "discovery.type=single-node" elasticsearch:7.5.1

docker run -p 9800:9800 --network elk --link elasticsearch:demo containerize/elastichd 


docker run --name elasticsearch elasticsearch:7.5.1


http.cors.enabled: true
http.cors.allow-origin: "*"