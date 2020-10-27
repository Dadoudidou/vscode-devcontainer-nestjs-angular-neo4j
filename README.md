# Template Dev Container NodeJS Neo4j

## Summary

Conteneur de développement proposant une instance nodejs et une instance neo4j

| Metadata                    | Value                                            |
| --------------------------- | ------------------------------------------------ |
| _Contributors_              | Dadoudidou                                       |
| _Definition type_           | Docker Compose                                   |
| _Works in Codespaces_       | Yes / No                                         |
| _Container host OS support_ | Linux, macOS, Windows                            |
| _Languages, platforms_      | JS, NEO4J                                        |


## Using this definition with an existing folder

**[Optional] Include any special setup requirements here. For example:**

While the definition itself works unmodified, you can select the version of **YOUR RUNTIME HERE** the container uses by updating the `VARIANT` arg in the included `.devcontainer/docker-compose.yml` file.

```yaml
args:
  VARIANT: buster
```

### Adding another service

You can add other services to your `docker-compose.yml` file [as described in Docker's documentation](https://docs.docker.com/compose/compose-file/#service-configuration-reference). However, if you want anything running in this service to be available in the container on localhost, or want to forward the service locally, be sure to add this line to the service config:

```yaml
# Runs the service on the same network as the app container, allows "forwardPorts" in devcontainer.json function.
network_mode: service:app
```

### Adding the definition to your project

1. If this is your first time using a development container, please follow the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started) to set up your machine.

2. To use VS Code's copy of this definition:

   1. Start VS Code and open your project folder.
   2. Press <kbd>F1</kbd> select and **Remote-Containers: Add Development Container Configuration Files...** from the command palette.
   3. Select the **YOUR NAME HERE** definition.

3. To use latest-and-greatest copy of this definition from the repository:

   1. Clone this repository.
   2. Copy the contents of this folder in the cloned repository to the root of your project folder.
   3. Start VS Code and open your project folder.

4. After following step 2 or 3, the contents of the `.devcontainer` folder in your project can be adapted to meet your needs.

5. Finally, press <kbd>F1</kbd> and run **Remote-Containers: Reopen Folder in Container** to start using the definition.

## [Optional] Testing the definition

This definition includes some test code that will help you verify it is working as expected on your system. Follow these steps:

1. If this is your first time using a development container, please follow the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started) to set up your machine.
2. Clone this repository.
3. Start VS Code, press <kbd>F1</kbd>, and select **Remote-Containers: Open Folder in Container...**
4. Select this folder from the cloned repository.
5. **[Provide any information on steps required to test the definition.]**

