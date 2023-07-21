
# Multicontainer App on Kubernetes 

## Introduction

This is a multi-container application on Kubernetes. The application consists of a client app, an Express server app, a worker app, a Redis database, and a PostgreSQL database. Each component is deployed as a separate Kubernetes deployment object, and the PostgreSQL database uses a persistent volume claim for data storage. Additionally, the application is exposed to external traffic through an Ingress service.

## Prerequisites

Before starting the deployment process, ensure you have the following prerequisites:

1. A running Kubernetes cluster.
2. `kubectl` command-line tool installed and configured to interact with the Kubernetes cluster.
3. `git` installed on your local machine.

## Steps to Deploy the Multicontainer App

Follow these steps to deploy the multicontainer app:

1. Clone the Repository:

   ```
   git clone https://github.com/amarachi2022/Kubernetes-App-Deployment.git
   cd Kubernetes-App-Deployment
   ```

2. Deploy the K8s directory: This folder contains all the configuration files for the multi-container app

   ```
   kubectl apply -f k8s
   ```

## Accessing the Application

Once the deployment is complete, you can access the client app through the Ingress service. Obtain the external IP of the Ingress service and access the application using a web browser.

