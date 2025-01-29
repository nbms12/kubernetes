Aim of project : Run nginx docker image on pod in minikube cluster , and make it accessible to outside world. 

requirements : 
1.install kubectl 
2.install minikube
3. latest nginx image


step1 : create deployment first , to run docker image 


![image](https://github.com/user-attachments/assets/b3932444-e7ba-45da-8fe2-25a8036b71e8)


step2 : Apply the service under tis node, in order to expose tis container to outside world 

![image](https://github.com/user-attachments/assets/1333e997-dca3-4a64-a4f7-b4d261b52413)


step3: Access the Application ,Get the URL to access the Nginx web server


![image](https://github.com/user-attachments/assets/81668b0d-87e6-4e43-9338-c9d1989a2782)






step5: open url in browser to access app .




![image](https://github.com/user-attachments/assets/02c68aef-fb50-4ec8-b4a2-bd78564d551a)






