# Docker installed inside of container 

In this method, we need to install Docker inside the agent container. The recommended approach is to run the Docker daemon (`dockerd`) in privileged mode.

## Prerequisites
- Ensure that the agent container has sufficient privileges to run Docker.
- Verify that the host machine has Docker installed and properly configured.

## Installation Steps

1.only start it whit docker compose 

```bash
$ sudo docker compose up --build
```

## Verification
To verify that Docker is installed and running correctly inside the agent container, execute the following command:

```bash
$ docker pull hello-world 
$ docker run hello-world 
```

If Docker is installed and functioning properly, you should see the output of hello-world image.

## Conclusion
By following these steps, you have successfully installed Docker inside the agent container. You can now utilize Docker to build, deploy, and manage containers within your environment.

Note: Running Docker in privileged mode grants extensive system-level access to the container, which may have security implications. Exercise caution and ensure that the agent container is adequately secured.