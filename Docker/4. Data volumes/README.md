# Data volumes

> There are `--mount` and `--volume (-v)` flags can be used in standalone containers since Docker 17.06 , check the [document](https://docs.docker.com/storage/volumes) for details.

## Mount a container's data volume

````
$ docker run -d --name xxx -v {/directory path} {image}[:tag]
````

ex.  Create an /app directory inside the container

```
$ docker run -d --name devtest -v /app nginx:latest
```

## Mount a local directory to container's data volume

Mount a local directory (if not exist, will create it) to the container,

```
$ docker run -d --name xxx -v {local directory path}:{/container directory path}[:rw|:ro] {image}[:tag]
```
|        Parameter        | in short | Value | Description |
|:------------------------|:--------:|:-----:|:------------|
| :rw |  | | Read and write, default value |
| :ro |  | | Read only |

ex.
```
$ docker run -d --name my-dev -v /jb/volume:/app:ro nginx:latest
```