In Kubernetes, an Ingress is an object that allows access to your Kubernetes services from outside the Kubernetes cluster. You configure access by creating a collection of 
rules that define which inbound connections reach which services.


![image](https://github.com/user-attachments/assets/7c6cf200-de56-4b73-95e0-5e3477bbe2e7)


Installation Guide
1.Start by creating the “mandatory” resources for Nginx Ingress in your cluster.

kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/master/deploy/mandatory.yaml


2.Then, enable the ingress add-on for Minikube.

minikube addons enable ingress


3.Creating a Kubernetes Ingress
First, let’s create two services to demonstrate how the Ingress routes our request. We’ll run two web applications that output a slightly different response.

a. apple-pod and with a service attached to it. 
b. banana-pod and with a service attached to it. 



