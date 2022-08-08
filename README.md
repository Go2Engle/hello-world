# Hello-World

## Deploy via Helm
Clone the repository locally to your PC and run the below command

```
helm install hello-world .\hello-world-chart\ --values .\hello-world-chart\values.yaml
```

> **Note** 
> To deploy into a specific namespace add `--namespace <name>` to the command above