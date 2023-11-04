# Docker


## Images

- [**WebP Server**: allows you to serve WebP images on the fly.](https://github.com/webp-sh/webp_server_go)



## Download the image from the Docker register

```sh
docker pull imagename
```

## Installed images list

```sh
docker images
```

## Performs the image

```sh
docker run imagename
```

## Performs the image and enters the Docker console

```sh
docker run -it imagename sh
```

## Performs the image by detaching from the terminal, exposing random doors, giving a name to the container

```sh
docker run -d -P --name static-site imagename
```

## Performs the image by assigning public doors

```sh
docker run -p 8888:80 imagename
```

## Shows the doors of a container through the name assigned

```sh
docker port static-site
```

## Finish a container via the assigned name

```sh
docker stop static-site
```

## Show containers in execution

```sh
docker ps
```

## Show containers in executed

```sh
docker ps -a
```

## Delete a container performed

```sh
docker rm containerId
```

## Delete all containers exited

```sh
docker rm $(docker ps -a -q -f status=exited)
```

## Delete all containers

```sh
docker container prune
```

## Fill out an image by specifying a name tag and indicating the location

```sh
docker build -t imagename .
```
