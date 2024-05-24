# Blog Hub


## Steps for reproducing:

Step 1. Clone the project
`
git clone https://github.com/1Shubham7/BlogHub.git
`

Step 2. Install the required dependencies

`npm i`

Step 3. Now you can simply see it running locally using the following command:

`npm start`

Step 4. You can either run the image where I have containerized this application:

`docker run -p 8080:80 1shubham7/react-helm-tutorial:1.0.0`

Or better, we can create a local Kubernetes cluster and deploy the application there. For that first create a Kubernetes cluster using Minikube:

`minikube start`

Step 6. Install the Helm chart that we have created:

`helm install --dry-run react-chart ./charts/react-chart`

Step 7. And now we can port-forward our Kubernetes service "reach-chart to the port 8000:

`kubectl port-forward svc/react-chart 8000:80`

And with that we will have our blog application running in the `localhost:8000` of our machine:

![image](https://github.com/1Shubham7/BlogHub/assets/116020663/423ea939-8090-4ace-a237-2c0db2a6c841)
