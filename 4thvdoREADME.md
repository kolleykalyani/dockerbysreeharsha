### Multistage Docekr file :

* A **multi-stage Dockerfile** is a way to optimize Docker images by using multiple **FROM** instructions in one Dockerfile. This technique helps reduce the final image size by copying only the necessary artifacts (like binaries, libraries, or executables) from one stage to another, avoiding unnecessary build tools and dependencies in the final image.

### Docker volumes :

* A **Docker volume** is a storage mechanism in Docker that allows data to persist beyond the life of a container. It is used to store data that is generated and used by Docker containers, and it ensures that data can be shared between containers or persisted after a container stops or is removed.

* If you’re running a database in a Docker container and want to ensure the data persists even if the container stops, we can use a Docker volume.

* To list the docker volumes

```
docker volume ls
```

* To create a docker volume

```
docker volume create my_volume
```

* To inspect the volume

```
docker volume inspect my_volume
```

* 
