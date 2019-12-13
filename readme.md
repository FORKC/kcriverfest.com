# KC Riverfest
> The public site for [KC Riverfest](https://kcriverfest.com). Brought to you by [Friends of the River Kansas City](https://forkc.org).

# Contributing

Visit the public repository on [GitHub](https://github.com/FORKC/kcriverfest.com) to submit issues or clone for development.

## Containers and orchestration

We recommend [Docker](https://docs.docker.com/) and [skaffold](https://skaffold.dev/) to create the local development environment matching deployments.
You can use already included docker files to build an image, and skaffold to load them into [Kubernetes](https://kubernetes.io/).

Ensure you've download and installed Docker, and check on the option to install Kubernetes locally.
Ensure you've install skaffold.

From there, start bash or powershall as needed at the root and run `skaffold dev` which will load a deployment and a service bound to [localhost:8080](http://localhost:8080) and refreshed with each code change.

## Publishing the image and updating production

Eventual nodes, but it's not working yet:
```bash
docker build -t kcriverfest .
```
