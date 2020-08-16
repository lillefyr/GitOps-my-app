# My App

Build:

```
GOOS=linux GOARCH=amd64 go build .
docker build -t my-app .
```

Run:

```
docker run -e GREETING=Howdy my-app
```

### Release:

```
docker login
docker tag my-app ariedeldocker/my-app
docker push ariedeldocker/my-app
```

### Clean Up

```
docker rmi my-app
```
