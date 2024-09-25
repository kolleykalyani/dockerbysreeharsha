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

  
