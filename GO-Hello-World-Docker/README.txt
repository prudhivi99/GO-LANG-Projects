docker build -t hello-docker .

docker tag hello-docker prawin24/hello-docker:latest
docker tag hello-docker prawin24/golang-hello-docker:latest

docker login -u "prawin24" -p "" docker.io

docker push prawin24/golang-hello-docker:latest

docker run -d  prawin24/golang-hello-docker
docker run prawin24/golang-hello-docker