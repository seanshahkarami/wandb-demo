# Weights and Biases Sage Demo

This is an example deployment of a Weights and Biases publisher app.

First, add a `wand-api-key` secret with your `WANDB_API_TOKEN`:

```sh
kubectl create secret generic wand-api-key --from-literal=WANDB_API_KEY=YOURAPIKEY
```

The deploy the job:

```sh
kubectl apply -f job.yaml
```

To delete the job:

```sh
kubectl delete -f job.yaml
```

To view the logs:

```sh
kubectl logs -f jobs/wandb-demo
```
