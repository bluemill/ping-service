# Ping service

This is a tiny utility for pinging a list of provided URLs over and over. It was built to run inside of a Kubernetes cluster to watch a list of internal service endpoints during network upgrades.

## Usage

You can apply the `ping-service.yaml` file directly to have it ping `https://google.com` as an example. To customize, download the file and update the `PING_URLS` environment variable.
```shell
kubectl apply -f ./ping-service.yaml
kubectl logs -f [name]
```