# Helm Fun

Playing around with Helm in Minikube

## Usage

### Setup

- [Install VirtualBox, kubectl, and minikube](https://kubernetes.io/docs/setup/minikube)
- Launch minikube `minikube start`
- Ensure your minikube cluster is working `kubectl cluster-info`
- Initialize Helm and install Tiller `helm init`

### Working with Helm charts and releases

```shell
helm install --debug --dry-run ./mychart
helm install ./mychart
helm upgrade <release-name> ./mychart
helm ls
helm get manifest <release-name>
helm delete <release-name>
```
