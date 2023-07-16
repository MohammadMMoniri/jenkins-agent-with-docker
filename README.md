# Jenkins Agent with Docker

This repository provides various ways to use Docker with Jenkins agents.

## Introduction

Jenkins is a popular open-source automation server that allows you to automate various tasks, including building, testing, and deploying software. Jenkins agents are responsible for executing the jobs or tasks defined in Jenkins.

Docker is a containerization platform that allows you to package applications and their dependencies into lightweight, portable containers. Using Docker with Jenkins agents can provide several benefits, such as isolation, reproducibility, and scalability.

## Getting Started

To get started with using Docker with Jenkins agents, follow these steps:

1. Clone this repository: `git clone https://github.com/mohammadmmoniri/jenkins-agent-with-docker.git`
2. Install Docker on your machine if you haven't already. Refer to the official Docker documentation for installation instructions specific to your operating system.
3. Choose one of the methods provided in this repository for running Jenkins agents with Docker.
4. Follow the instructions in the respective method's directory to set up and configure the Jenkins agent using Docker.
5. Run the Jenkins agent container and connect it to your Jenkins server.
6. Start running your Jenkins jobs using the Docker-based agent.

## Methods

This repository provides the following methods for using Docker with Jenkins agents:

1. Method 1: Docker-in-Docker (DinD)
   - This method involves running a Jenkins agent container with Docker installed inside it. It allows you to run Docker commands and build Docker images within the agent container.
   - See the `method1-dind` directory for detailed instructions.

2. Method 2: Docker Socket Sharing
   - This method involves sharing the Docker socket from the host machine with the Jenkins agent container. It allows the agent to communicate directly with the Docker daemon on the host.
   - See the `method2-docker-socket-sharing` directory for detailed instructions.

Choose the method that best suits your requirements and follow the instructions provided in the respective directory.

## Contributing

If you would like to contribute to this repository, please follow these guidelines:

1. Fork the repository.
2. Create a new branch for your feature or bug fix: `git checkout -b my-feature`.
3. Make your changes and commit them with descriptive commit messages.
4. Push your changes to your forked repository.
5. Submit a pull request detailing your changes.

## License

This repository is licensed under the [MIT License](LICENSE). Feel free to use and modify the code as per your needs.

## Acknowledgements

We would like to thank the Jenkins and Docker communities for their excellent documentation and resources that helped in creating this repository.

Happy Jenkins automation with Docker!