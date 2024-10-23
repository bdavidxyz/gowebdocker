# Simplest go web server with Docker

Check go is installed on your machine with `go version`

In your terminal run

```shell
go run app.go
```

```shell
docker build -t gowebdocker .
```

```shell
docker run -d -p 8080:80 --name gowebdocker gowebdocker
```


