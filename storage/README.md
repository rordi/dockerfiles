Storage Dockerfile
------------------

This Dockerfile creates a Docker image which will, by default, mount a /data volume to be used
by other containers in the Docker network.

You can define additional volumes in your docker-compose.yml file.


~~~~
  data:
    domainname: local
    container_name: data
    image: rordi/docker-storage:latest
    volumes:
      # additional volume mounts
      - ./dummy/data:/home/dummy/data
~~~~
