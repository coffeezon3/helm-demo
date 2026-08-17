# Helm Demo – Kubernetes

This project is part of the **Tech With Nana DevOps Bootcamp**.

The goal of this project was to deploy an application to Kubernetes using **Helm**. I used Minikube as the local Kubernetes cluster and deployed MongoDB and Mongo Express.

## Technologies

* Kubernetes
* Minikube
* Helm
* Docker
* MongoDB
* Mongo Express

## What I did

In this project I:

* started a local Kubernetes cluster with Minikube
* created Kubernetes resources for MongoDB
* deployed MongoDB to Kubernetes
* deployed Mongo Express
* configured services for the applications
* configured an Ingress for Mongo Express
* used Helm to manage the Kubernetes deployment
* rendered the Helm templates to check the generated Kubernetes YAML
* tested the deployment with `kubectl`
* accessed Mongo Express through the configured hostname

## Project files

Some of the important files in this repository are:

* `helm-ingress.yaml` – Ingress configuration
* `rendered-mongodb.yaml` – rendered Kubernetes configuration
* Helm configuration files used for the deployment

## Setup

Start Minikube:

```bash
minikube start
```

Check the cluster:

```bash
kubectl get nodes
```

Check the running pods:

```bash
kubectl get pods
```

Check the services:

```bash
kubectl get services
```

Check the Ingress:

```bash
kubectl get ingress
```

## Helm

I used Helm to render and deploy the Kubernetes configuration.

To check the Helm releases:

```bash
helm list
```

The generated Kubernetes configuration can also be checked with Helm template rendering.

Example:

```bash
helm template ...
```

## Verification

After deploying the application, I checked the Kubernetes resources with `kubectl`.

The main things I verified were:

* Kubernetes cluster is running
* MongoDB pod is running
* Mongo Express pod is running
* Kubernetes services are available
* Ingress is configured
* Mongo Express can be accessed through the configured hostname

Mongo Express was tested through:

```text
http://mongo-express.local
```

## Screenshots

Screenshots showing the deployment and verification can be found in the `screenshots` folder.

Examples:

* Minikube running
* Kubernetes pods
* Kubernetes services
* Helm release
* Ingress
* Mongo Express in the browser

## What I learned

This project helped me understand how Helm can be used to manage Kubernetes resources instead of creating every Kubernetes manifest manually.

I also practiced working with Minikube, `kubectl`, Kubernetes Services and Ingress.

## Course

Tech With Nana – DevOps Bootcamp

Module: Kubernetes / Helm
