# Django App

This is a Django Hello World app. It contains a simple html page with an image being picked up from the internet proving the networking works fine from inside the pod and onto the internet via nat gateway > internet gateway making the application secure.

## CircleCI CI/CD

Changes made inside this dir will result in a new deployment to kick in in CircleCI. All the deployments are rolling and the application can be accessed via the ALB.

## Kubernetes Deployment

The k8s folder consist of a Deployment and Service yaml files. A load balancer service is provisioned and 3 Pods in different avaialbilty zones are deployed.