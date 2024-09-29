### What is Dockerfile ?

* Dockerfile is nothing but set of instructions.

* Some of the instructions are :

* ADD		        :  Add local or remote files and directories.
 
* ARG		        :  Use build-time variables.
 
* CMD		        :  Specify default commands.
 
* COPY	        :  Copy files and directories.
 
* ENTRYPOINT	  :  Specify default executable.

* ENV		        :  Set environment variables.

* EXPOSE		     :  Describe which ports your application is listening on.

* FROM	        :	 Create a new build stage from a base image.

* HEALTHCHECK  :  Check a container's health on start up.

* LABEL        :  Add metadata to an image.

* MAINTAINER   :  Specify the author of an image.

* ONBUILD	     :	 Specify instructions for when the image is used in a build.

* RUN	         :  Execute build commands.

* SHELL        :	 Set the default shell of an image.

* STOPSIGNAL	  :  Specify the system call signal for exiting a container.

* USER	        :	 Set user and group ID.

* VOLUME	      :	 Create volume mounts.

* WORKDIR	     :  Change working directory.


* To see all the processes or steps running while building the images

```
docker run -rm -d --name kalyani -p 8000:80 imagename --progress=plain
```

### What is Container ?

* The word “**container**” doesn’t mean anything super precise. Basically, there are a few new Linux kernel features (“**namespaces” and “cgroups**”) that let you isolate processes from each other. When you use those features, you call it “**containers**”.

* Basically, these features let you pretend you have something like a virtual machine, except it’s not a virtual machine at all, it’s just processes running in the same Linux kernel. 

