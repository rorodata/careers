# Problem Set for Devops
### Write back to us with your solution repo raghav [at] rorodata [dot] com
### More details [here](https://angel.co/rorodata/jobs/283569-devops-engineer)

**Problem: Build a web dashboard for docker**
Write a web application in *Python* that uses the docker API to find out the current running Docker containers and available images. The web app should have the following pages:
- one page to list all the active containers
- one page to list all available images
- one page for each container
- one page for each image

It should allow the following actions:
- stop a running container
- delete an existing image
- add a new image
- start a new container [it should prompt for the command to run and ports to
expose]
- look at logs of a running container

Also, provide a script to provision the server and deploy this application on a remote machine. There should be a ReadME with instructions about how to provision the server and deploy the application. Ideally, each of them should be just a single command.


Feel free make any assumptions about the details that are not mentioned here.

