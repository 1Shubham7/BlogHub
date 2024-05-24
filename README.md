# Blog Hub

Blog Hub is a platform designed to help you discover the best blogs from reputable authors across the globe on any topic in the field of technology. It is a React application containerized using Docker and deployed on Kubernetes along with Helm charts to manage it.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Running Locally](#running-locally)
- [Running with Docker](#running-with-docker)
- [Deploying to Kubernetes](#deploying-to-kubernetes)

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)
- [Docker](https://www.docker.com/)
- [Kubernetes](https://kubernetes.io/)
- [Minikube](https://minikube.sigs.k8s.io/docs/start/)
- [Helm](https://helm.sh/)

## Getting Started

To get a local copy of the project up and running, follow these steps:

### Step 1: Clone the Repository

```sh
git clone https://github.com/1Shubham7/BlogHub.git
cd BlogHub
```

### Step 2: Install Dependencies

Install the required dependencies using npm:

```sh
npm install
```

### Step 3. Running Locally

Now you can simply see it running locally using the following command:

```sh
npm start
```

The application will be accessible at `http://localhost:3000`.

### Step 4. Running with Docker

To run the containerized application, use Docker:

```sh
docker run -p 8080:80 1shubham7/react-helm-tutorial:1.0.0
```

The application will be accessible at `http://localhost:3000`. Or better, we can create a local Kubernetes cluster and deploy the application there. For that first create a Kubernetes cluster using Minikube:

### Step 5. Deploying to Kubernetes

- Create a local Kubernetes cluster using Minikube:

```sh
minikube start
```

- Install the Helm chart for the application:

```sh
helm install --dry-run react-chart ./charts/react-chart
```

- And now you can port-forward the Kubernetes service "reach-chart to the port 8000:

```sh
kubectl port-forward svc/react-chart 8000:80
```

And with that we will have our blog application running in the `localhost:8000` of our machine:

![image](https://github.com/1Shubham7/BlogHub/assets/116020663/423ea939-8090-4ace-a237-2c0db2a6c841)
