# Simplest go web server with Docker

## Check Go version

Check go is installed on your machine with `go version`

## Run simple web app


In your terminal run

```shell
sudo go run app.go
```

And display localhost:80 in your web browser, to check that everything is ok.

## Build the docker image

Now, go back to your terminal, and stop the local web server.

Build the docker image with :

```shell
docker build -t gowebdockerimage .
```

## Launch the docker container

And launch the container with  :

```shell
docker run -d -p 8080:80 --name gowebdockercontainer gowebdockerimage
```

And display localhost:8080 in your web browser, to check that everything is ok.
Note that localhost:80 is NOT anymore reachable, because it's running inside the docker container.

Stop the container with

```shell
docker container stop gowebdockercontainer
```