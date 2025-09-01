# tmux-devcontainers-examples
A repository of examples for testing the [tmux-devcontainers](https://github.com/phil/tmux-devcontainers) plugin
A repository of examples for testing tmux-devcontainers plugin

With DevContainers, there are four main types of configurations you can use to set up your development environment. For the tmux-devcontainers plugin, we have created example projects to test the status bar and menu functionalities for each configuration type.

## Docker Compose (single)

For single compose setup, we expect the status to show each service and its status.

```
# #{devcontainers_workspace}
DockerComposeSingleExampleProject

# #{devcontainers_status}
app:running database:running
```

## Docker Compose (double)

For a double compose setup, we expect the status to show each service from both compose files and their status.

```
# #{devcontainers_workspace}
DockerComposeExampleProject

# #{devcontainers_status}
app:running database:running cache:running 
```

## Dockerfile

For a Dockerfile setup, we expect the status to show "Dockerfile" and its status.

```
# #{devcontainers_workspace}
DockerFileExampleProject

# #{devcontainers_status}
Dockerfile:running
```

## Image

For an image setup, we expect the status to show the image name and its status.

```
# #{devcontainers_workspace}
RubyImageExampleProject

# #{devcontainers_status}
ruby:1-3.4-bullseye:running
```
