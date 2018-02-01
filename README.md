Development environment for AGILE
=================================

This repository gathers a consistent set of all the code needed to compile and run AGILE from source.

Usage
-----

- Make sure all git submodules are checked out
```
git submodule update --init --recursive
```

- Configure agile-stack to use docker's local build feature
```
cp agile-stack/docker-compose.override.yml.buildall agile-stack/docker-compose.override.yml
```

- Configure agile-stack for your local environment by creating and modifying agile-stack/.env
```
cd agile-stack
cp .env.example .env
vi .env
```

- Build all the docker containers (and take a long coffe break)
```
docker-compose build

```

- run AGILE as usual: check the README of agile-stack.
