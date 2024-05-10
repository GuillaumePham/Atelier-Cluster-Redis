# Atelier-Cluster-Redis


##Etape 1##
Création d'un conteneur avec une image en ligne docker
docker run --name my-redis-container -d redis
##Etape 2##
Création d'un cluster (réseau)
docker network create redis-net
##Etape 3##
docker pull redis
##Etape 4##
docker run -d --name redis1 --net redis-net redis
docker run -d --name redis2 --net redis-net redis
docker run -d --name redis3 --net redis-net redis
##Etape 5##
docker container ls

