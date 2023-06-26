# Udacity Cloud DevOps Engineer Nanodegree Capstone Project

A web application that provides a link to the Udacity website for visitors. It's an example of a CI/CD pipeline to demonstrate what I've learned in my Udacity nanodegree program.

## NPM Scripts

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

## Linters

### `npx eslint ./src`
Run ESLint against the source directory

### `docker run --rm -i hadolint/hadolint < Dockerfile`
Run hadolint against the Dockerfile

## Kubernetes Manual Setup

### `eksctl create cluster -f .eksctl-config.yml`
Create the Kubernetes cluster in AWS using CloudFormation\
The cluster consists of two t2.micro (free tier) EC2 instances

### `kubectl create -f .kubectl-loadbalancer.yml`
Create a load balancer for the pod

### `kubectl get nodes,services`
Verify the nodes and load balancer are running\
Get the public URL for this application


