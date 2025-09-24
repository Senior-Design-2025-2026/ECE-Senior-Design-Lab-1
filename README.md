# ECE-Senior-Design-Lab-1

## System Architecture

## Pin Out

## Finished Product 
### Thermostat Box
### Dashboard

# Running the Project
## Required installations:
To run this project, you must have docker installed on your computer. Please read the [Docker documentation](https://docs.docker.com/) on how to get started.

## IMPORTANT: using git submodules
It is required that you run this command to use the containerized version of Lab 1. This pulls the other repositories (web server, embedded code, celery worker, dummy stream writer) 

After pulling this repository, run the following command:
```
git submodule update --init L1-testing-redis-stream-writer
```

If there are any issues and a repository is not pulled, target each repository individually until fixed:
ex: initializing the testing stream writer repository
```
git submodule update --init L1-testing-redis-stream-writer
```

## Running Project:
```
TBD (need to define modes)
```

## Running in (Test Mode):
Although you likely do not have the physical box with thermometers, you can still run the web-server by using the following commands:

```
TBD (need to define modes)
```

