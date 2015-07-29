## MuleESB Docker Image

This repo contains docker image for [MuleESB](http://www.mulesoft.org).

You need to pull `Mule` docker image from Docker registry via command below :

```
docker pull eddumelendez/mule
```

After that you should be able to run `Mule` docker image by :

```
docker run -ti eddumelendez/mule
```

## Dockerize your mule app

```
FROM eddumelendez/mule
ADD mule-app.zip $MULE_HOME/apps/
EXPOSE 8081:8081
```

After creating the Dockerfile you need to build it. You can build your Dockerfile with the command below :

```
docker build .
```
