# TinkerWare Spring Environments

This is a TinkerWare repository to manage spring enviroments.

You will be able to do quick software development. 

Here are some things that you should keep in mind:

You can start doing code changes inside `project`. There's where your code lives
and it will be shared automatically with the inner container. 
It will be running through the shared port `8090`. 

Follow the following commands to be able to develop easily (Described below):

`./tinker start`
`./tinker restart`
`./tinker restart --force`
`./tinker stop`

**Requeriments:**

- Linux/MacOS enviroment
- docker

**tinker Usage**

`./tinker start`

If its the first run it will create the docker enviroment this may take a few minutes 
when its done, and every execution after that it's going to run spring-boot:run
using the docker enviroment and send the output of the  project to the terminal, 
if you have a working project you can open [GitHub Pages](http://localhost:8090/) to see it working.


`./tinker restart`

When making changes to your code, restarts the execution to test the changes

`./tinker restart --force`

use only if restart doesn't show the changes made to the code

`./tinker stop`

stops the runing instance of the container
