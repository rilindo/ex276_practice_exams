Course Objectives:

# Reference URLs:

- https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux_atomic_host/7/html-single/getting_started_with_containers/
- https://docs.docker.com/edge/engine/reference/commandline/docker/

# Implementing images

- Understand and use FROM (the concept of a base image) 
  - https://docs.docker.com/engine/reference/builder/#from
- Understand and use RUN 
  - https://docs.docker.com/engine/reference/builder/#run
- Understand and use ADD 
  - https://docs.docker.com/engine/reference/builder/#add
- Understand and use COPY 
  - https://docs.docker.com/engine/reference/builder/#copy
- Understand the difference between ADD & COPY 
  - https://stackoverflow.com/questions/24958140/what-is-the-difference-between-the-copy-and-add-commands-in-a-dockerfile
- Understand and use WORKDIR and USER 
  - https://docs.docker.com/engine/reference/builder/#workdir
  - https://docs.docker.com/engine/reference/builder/#user
  - Understand security-related topics
- Understand the differences and applicability of CMD versus ENTRYPOINT
  - https://docs.docker.com/engine/reference/builder/#cmd
  - https://docs.docker.com/engine/reference/builder/#entrypoint
  understand
  - Understand ENTRYPOINT with param
- Understand and use ONBUILD
  - https://docs.docker.com/engine/reference/builder/#onbuild
- Understand when and how to EXPOSE port from a Dockerfile
  - https://docs.docker.com/engine/reference/builder/#expose
- Understand and use environment variables inside images
  - Understand how ENV is used to allow multiple containers work together
    - https://docs.docker.com/engine/reference/builder/#env
- Understand container VOLUME
  - https://docs.docker.com/engine/reference/builder/#volume
  - Mount a host directory as a data volume
     - Understand security and permissions requirement related to this approach
  - Create and mount a data volume container
     - https://docs.docker.com/engine/reference/commandline/volume_create/
     - Understand lifecycle and "clean up" requirement of this approach
       - https://docs.docker.com/engine/reference/commandline/volume_prune/
       - https://docs.docker.com/engine/reference/commandline/volume_rm/

# Managing images

- Understand private registry security
  - https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux_atomic_host/7/html-single/getting_started_with_containers/#creating_a_private_docker_registry_optional
- Interact with many different registries
  - https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux_atomic_host/7/html-single/getting_started_with_containers/#getting_images_from_remote_docker_registries
- Understand and use image tags
  - https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux_atomic_host/7/html-single/getting_started_with_containers/#tagging_images
  - https://docs.docker.com/engine/reference/commandline/tag/
  
- Push and pull images from/to registries
  - https://docs.docker.com/engine/reference/commandline/push/
  - https://docs.docker.com/engine/reference/commandline/pull/
- Backup an image with its layers and meta datas versus backup a container state
  - https://docs.docker.com/engine/reference/commandline/save/

# Running containers locally

- Link containers
  - https://docs.docker.com/engine/reference/commandline/save/
  https://docs.docker.com/engine/userguide/networking/
  https://docs.docker.com/engine/userguide/networking/default_network/dockerlinks/
  - Connect with the linking system
  - Understand and apply environment variables naming requirement while using the linking system
- Get container logs
  - https://docs.docker.com/engine/reference/commandline/logs/
- Listen to Docker events on the Docker host
  - https://docs.docker.com/engine/reference/commandline/events/
- Use Docker inspect
  - https://docs.docker.com/engine/reference/commandline/inspect/
- Share data between containers
  - Use a mounted host directory as a data volume
    - https://docs.docker.com/engine/reference/commandline/run/#mount-volume--v-read-only
  - Use and mount a data volume container
  - https://docs.docker.com/engine/reference/commandline/run/#add-bind-mounts-or-volumes-using-the-mount-flag
- Understand host and container basic security best practices