# Kubernetes Practice

## Commands

- minikube start

- kubectl get nodes
- kubectl create deployment [name] --image=[image-name]
- kubectl get all
- kubectl get deployments
- kubectl get replicasets
- kubectl edit deployment [deployment-name]
- kubectl delete deployment [deployment-name]

## Pods

- kubectl get pods
- kubectl get pod -o wide
- kubectl describe pod [pod-name]
- kubectl get pod --watch
- kubectl exec -it [pod-name] -- bin/bash
- kubectl log [pod-name]

## Using configuration files

### Deployment configurations

- kubectl apply -f [deployment-file.yaml] (same for update)
- kubectl delete -f [deployment-file.yaml]
- kubectl get deployments [deployment-name] -o yaml > [output-result.yaml]

### Service configurations

- kubectl apply -f [service-file.yaml] (same for update)
- kubectl delete -f [service-file.yaml]
- kubectl get services
- kubectl describe service [service-name]

### Secret configurations

- kubectl apply -f [secret-file.yaml] (same for update)
- kubectl delete -f [secret-file.yaml]
- kubectl get secrets

### Configs map configurations

- kubectl apply -f [config-map.yaml] (same for update)
- kubectl delete -f [config-map.yaml]
- kubectl get configmaps

### Namespaces

- kubectl get namespace
- Kubectl create namespace [name]
