In Kubernetes, an Ingress is an object that allows access to your Kubernetes services from outside the Kubernetes cluster. You configure access by creating a collection of 
rules that define which inbound connections reach which services.


![image](https://github.com/user-attachments/assets/7c6cf200-de56-4b73-95e0-5e3477bbe2e7)


#Installation Guide

1.Start by creating the “mandatory” resources for Nginx Ingress in your cluster.

kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/master/deploy/mandatory.yaml


2.Then, enable the ingress add-on for Minikube.

minikube addons enable ingress


3.Creating a Kubernetes Ingress

First, let’s create two services to demonstrate how the Ingress routes our request. We’ll run two web applications that output a slightly different response.

a. apple-pod and with a service attached to it. 

b. banana-pod and with a service attached to it. 


4. create Ingress
   
![image](https://github.com/user-attachments/assets/75bf196c-5d43-49de-8131-ecfadc48f8a8)


5. route to apple and banana service with respective paths

   ![image](https://github.com/user-attachments/assets/873a213d-3639-4657-b10f-f4c124120bb7)



   ![image](https://github.com/user-attachments/assets/e79decc0-c997-4a7b-b13e-be2478dbbcd1)



   



