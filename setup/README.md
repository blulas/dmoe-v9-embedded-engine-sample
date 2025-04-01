# IBM Business Automation Manager Open Editions - Setup Instructions - Docker Compose
If you are currently running docker, podman, or Rancher Desktop, you can utilize the docker compose configuration scripts in this section of the repository.  You can use `Docker Compose` to run the BAMOE images locally and the easiest way is to use `Rancher Desktop`.  Click [here](https://docs.rancherdesktop.io/getting-started/installation/) in order to get instructions on how to install Rancher Desktop in Docker mode.  

## Maven Repository
For more information on how to properly setup Maven for local development, visit [Setting Up Maven](./maven/README.md).

## Container Images
In order to setup Maven and other infrastructure services, you can use the supplied `docker-compose.yml` file, located in the root of the `setup` folder.  In order to install all services, simply open a terminal, go the repository `setup` folder, and type the following:

```
 docker compose up
```

or for a specific service in the `docker-compose.yml` file...

```
 docker compose up [optional]<service-name>
```

3.  The images will start containers on the following ports:

    | Service                   | Port @ localhost              |
    | ------------------------- | ----------------------------- |
    | BAMOE Maven               | [9020](http://localhost:9020) |
    | BAMOE Canvas              | [9090](http://localhost:9090) |







