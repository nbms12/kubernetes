Network Policies are a mechanism for controlling network traffic flow in Kubernetes clusters. They allow you to define which of your Pods are allowed to exchange network traffic. You should use them in your clusters to prevent apps from reaching each other over the network, which will help limit the damage if one of your apps is compromised.



There are three different ways to identify target endpoints:

1.Specific Pods (Pods matching a label are allowed)

2.Specific Namespaces (all Pods in the namespace are allowed)

3.IP address blocks (endpoints with an IP address in the block are allowed)



first lets create a two pods 

kubectl run qa-pod --image nginx:latest -l app=qa-pod 

kubectl run db-pod --image nginx:latest -l app=db-pod


![image](https://github.com/user-attachments/assets/2976b4dc-6fc6-4351-abc3-d8a4d6ffccd8)



now lets see communication of qa-pod to db-pod, 


![image](https://github.com/user-attachments/assets/bd412c89-08fb-495e-998d-e382e3b60cba)


they are talkin each other. our aim is to build security wall against db-pod who are in access by qa-pod. 






