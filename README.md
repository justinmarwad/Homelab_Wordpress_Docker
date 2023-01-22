# Wordpress Docker Compose Setup #

Setup Wordpress with Docker Compose in my homelab for fun and decided that I would publish this for anyone else who might find it useful.


## Setup ## 

### Technology ###

This setup is based on the [official Wordpress Docker image](https://hub.docker.com/_/wordpress/) and I have also included a [MariaDB](https://hub.docker.com/_/mariadb/) container for the database. Obviously, you will need to have Docker and Docker Compose installed on your system.

### Configuration ###

You will need to copy the `.env.example` file and name it `.env`. You will then need change the variables to ones that make sense. 

### Running ###

Once you have configured the `.env` file, you can run the following command to start the containers:

```bash
docker-compose up -d
```

Very simple and easy to get up and running.

## Notes/TODO ##

- I plan to convert this setup to Docker Swarm using Docker Stack to run this Compose file. In addition, I plan to leverage GlusterFS to have highly available storage for the wordpress and database data directories. I will update this README when I have completed these tasks. 
- I also plan on converting this to use Kubernetes in the future and that repository will be linked here when it is completed.
