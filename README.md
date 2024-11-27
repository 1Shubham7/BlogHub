<div align="center">
  <h1>Blog Hub - Know what's new in tech</h1>

  [![GitHub last commit](https://img.shields.io/github/last-commit/1Shubham7/BlogHub)](#)
  ![GitHub language count](https://img.shields.io/github/languages/count/1Shubham7/BlogHub)
  ![GitHub top language](https://img.shields.io/github/languages/top/1Shubham7/BlogHub)

</div>

Blog Hub is a platform designed to help you discover the best blogs from reputable authors across the globe on any topic in the field of technology. It is a React application containerized using Docker and deployed on Kubernetes along with Helm charts to manage it.

⭐ Star us on GitHub — it motivates me a lot!

[![Share](https://img.shields.io/badge/share-000000?logo=x&logoColor=white)](https://x.com/intent/tweet?text=Check%20out%20this%20project%20on%20GitHub:%20https://github.com/1Shubham7/BlogHub%20%23OpenIDConnect%20%23Security%20%23Authentication)
[![Share](https://img.shields.io/badge/share-1877F2?logo=facebook&logoColor=white)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/1Shubham7/BlogHub)
[![Share](https://img.shields.io/badge/share-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/sharing/share-offsite/?url=https://github.com/1Shubham7/BlogHub)
[![Share](https://img.shields.io/badge/share-FF4500?logo=reddit&logoColor=white)](https://www.reddit.com/submit?title=Check%20out%20this%20project%20on%20GitHub:%20https://github.com/1Shubham7/BlogHub)
[![Share](https://img.shields.io/badge/share-0088CC?logo=telegram&logoColor=white)](https://t.me/share/url?url=https://github.com/1Shubham7/BlogHub&text=Check%20out%20this%20project%20on%20GitHub)

## 📚Tech Stack


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

## 🤝 Contributing
  ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/1shubham7/BlogHub)
  ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-closed/1shubham7/BlogHub)
  ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr/1shubham7/BlogHub) 
  ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr-closed/1shubham7/BlogHub) 

Whether you have feedback on features, have encountered any bugs, or have suggestions for enhancements, we're eager to hear from you. Your insights help us make our application more robust and user-friendly. Please feel free to contribute by [submitting an issue](https://github.com/1Shubham7/BlogHub/issues) or [joining the discussions](https://github.com/orgs/Abblix/discussions). Each contribution helps us grow and improve. If you would like to contribute to this project, please read the [Contribution guidelines](CONTRIBUTING.md) and make sure to follow the [Code Of Conduct](CODE_OF_CONDUCT.md).
