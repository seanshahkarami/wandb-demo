# Weights and Biases Sage Demo

This is an example deployment of a Weights and Biases publisher app.

Once you have access to a development node, you'll need to do the one time step of adding a `wandb-api-key` secret with your `WANDB_API_KEY`:

```sh
kubectl create secret generic wandb-api-key --from-literal=WANDB_API_KEY=YOURAPIKEY
```

Now you can manage you job as follows:

```sh
# deploy the job
kubectl apply -f job.yaml

# get job status
kubectl get jobs

# get pod status
kubectl get pods

# tail the logs
kubectl logs -f jobs/wandb-demo

# delete the job when you're done
kubectl delete -f job.yaml
```

_Note: This demo is intentionally using only basic Kubernetes concepts and tooling to manage a single Job resource. In general, there are more tools like Kustomize or Helm which can go a long way in managing bigger examples._
