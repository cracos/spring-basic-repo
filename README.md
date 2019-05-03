
# TinkerWare Spring Environments

This is a TinkerWare repository to manage spring enviroments.

You will be able to do quick software development. 

Here are some things that you should keep in mind:

You can start doing code changes inside `project`. There's where your code lives
and it will be shared automatically with the inner container. 
It will be running through the shared port `8090`. 

Use the following commands to be able to develop easily (described below):

- `./tinker start`
- `./tinker restart`
- `./tinker restart --force`
- `./tinker stop`

**Requeriments:**

- Linux/MacOS enviroment
- docker installed
- A dockerID account already logged in with `docker login -u your_username`

**tinker file usage**

`./tinker start`

If its the first run it will create the docker enviroment and it may take a few minutes. 
When it's done, every execution after that it's going to run `spring-boot:run`
using the docker environment and send the output of the  project to the terminal, 
if you have a working project you can open the [default page](http://localhost:8090/) to see it working.


`./tinker restart`

When changes to your code were made, this restarts the execution to test them.

`./tinker restart --force`

Use only if `restart` doesn't show the changes made to the code.

`./tinker stop`

Stops the running instance of the container.
