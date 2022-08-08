# Hello-World
Simple hello-world application with nginx webserver serving a index.html page

## Build locally
To build locally clone the repository and run a docker build.
```
docker build .
```

This repository also contains a VScode devcontainer configuration that comes with tilt. Make sure you have VSCode with remote containers plugin enabled, docker installed, and a locally running k8s running. With those in place restart vscode in the container then run `tilt up` and follow instructions from the terminal.

> **Note**
> Tilt for this project is overkill and just here for example.

## Deploy via Helm
Clone the repository locally to your PC and run the below command

```
helm install hello-world .\hello-world-chart\ --values .\hello-world-chart\values.yaml
```

> **Note** 
> To deploy into a specific namespace add `--namespace <name>` to the command above