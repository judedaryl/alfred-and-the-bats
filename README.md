## alfred-and-the-bats

Container based CICD

<img src='https://github.com/judedaryl/alfred-and-the-bats/blob/main/AlfredAndTheBats.png?raw=true'/>


### Alfred

Orchestrator, Configuration Keeper

### Bats

Worker bats, does all the grunt work


### Build-Kits

Instruction sets for building

### Deploy where?

Anywhere


### Caching

Use a combination of Redis and s3. Redis to keep keys and track expirations, and s3 to store the actual files

### Redis

Redis will be used as a means of communication between the Orchestrator and the workers.
