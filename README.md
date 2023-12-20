# Weights and Biases Sage Demo

This is an example deployment of a Weights and Biases publisher app. All you need to do is provider your `WANDB_API_TOKEN` in the [kustomization.yaml](kustomization.yaml) file and run the following on a development node:

```sh
kubectl apply -k .
```
