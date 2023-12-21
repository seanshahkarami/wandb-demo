# Weights and Biases Sage Demo

This is an example deployment of a Weights and Biases publisher app.

First, add a `wand-api-key` secret with your `WANDB_API_TOKEN`:

```sh
kubectl create secret generic wand-api-key --from-literal=WANDB_API_KEY=YOURAPIKEY
```

The deploy the job:

```sh
kubectl apply -f .
```
