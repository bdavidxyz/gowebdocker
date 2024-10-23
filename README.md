# Simplest go web server with Docker

Check go is installed on your machine with `go version`

In your terminal run

```shell
sudo go run app.go
```

And display localhost:80 in your web browser, to check that everything is ok.

Now, go back to your terminal, and stop the local web server.

Build the docker image with :

```shell
docker build -t gowebdocker .
```

And launch the container with  :


```shell
docker run -d -p 8080:80 --name gowebdocker gowebdocker
```

And display localhost:8080 in your web browser, to check that everything is ok.

Stop the container with

```shell
docker container stop gowebdocker
```