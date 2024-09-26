### Difference b/w add and copy ? 

### Copy :
* It is used for copying files and directories from the host machine to a specific location in the Docker image.

* It can only copy files or directories from the build context.
 
* It's straightforward and predictable since it only copies files without any additional processing.

### Add :

* It also copies files and directories, but it provides extra features.

* Besides copying files, it can also handle URLs (downloads files from the web) and compressed files.

### When to use copy and add cmds ?

* Use **COPY** when you just need to copy files or directories into your Docker image.

* Use **ADD** when you need to extract archives or download files from remote locations.

### Dangling Images :

* Dangling images are untagged docker images that are not associated with any container.They are created when they overwritten with a new image with the same name and tag.

* To remove all dangling images

```
docker image prune
```

### Difference b/w CMD and ENTRYPOINT ?

* Both are same.Both are responsible for what the container should do when it is created.

* If we want to overridee the **CMD** we can do but we cannot override in the **ENTRYPOINT**.

* To see in which port the image is build or the container is running.

```
docker image inspect imageid
```

* 



  
