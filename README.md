# hello-mgo

## Goal
- Build distributed web application with mongo using mgo
- Dockerize golang mongo application

## Prerequisite
Docker

## Getting Started

Get repository from GitHub
```
git clone https://github.com/MasashiTeruya/hello-mgo.git && cd hello-mgo/app
```

Build Docker image
```
docker build -t hello-mgo .
```

Run MongoDB
```
docker run -d --name hello-mgo-mongo mongo
```

Run app
```
docker run -it --rm --link hello-mgo-mongo:mongo hello-mgo
```
