## alfred-and-the-bats

Container based CICD

<img src='https://github.com/judedaryl/alfred-and-the-bats/blob/main/AlfredAndTheBats.png?raw=true'/>


### Alfred

Orchestrator, Configuration Keeper

### Bats

Worker bats, does all the grunt work. Contains a docker-in-docker service, so that we can run builds in containers inside the container for isolation and to ensure consistent behavior of the scripts.


### Build-Kits

Instruction sets for building. Contains:
* detection script
* compilation script
  * tests
  * static code analysis
  * vulnerability analysis
  * compiling binaries
* deployment script
* specify docker image for each script????

### Deploy where?

Anywhere


### Caching

Use a combination of Redis and s3. Redis to keep keys and track expirations, and s3 to store the actual files

### Redis

Redis will be used as a means of communication between the Orchestrator and the workers.
