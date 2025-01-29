# kubernetes
repo is all about kubernetes 


Aim of project :  we will equipped knowledge on kubernetes tech. following topics ive gained skill and exposure 

 cluster ( as master node /control plane ) and 1 worker node is created while creating miniqube installation

 1. install kubectl ( as cli for kubernetes )

   
 3. install minikube ( u must have virtual box as that it creates an image to run  minikube in local machine ) 

    
      2.1 Invoke-WebRequest -OutFile 'c:\minikube\minikube.exe' -Uri 'https://github.com/kubernetes/minikube/releases/latest/download/minikube-windows-amd64.exe' -UseBasicParsing

    
      2.2  New-Item -Path 'c:\' -Name 'minikube' -ItemType Directory -Force

    
      2.3  $oldPath = [Environment]::GetEnvironmentVariable('Path', [EnvironmentVariableTarget]::Machine)

    
    if ($oldPath.Split(';') -inotcontains 'C:\minikube'){
               [Environment]::SetEnvironmentVariable('Path', $('{0};C:\minikube' -f $oldPath), [EnvironmentVariableTarget]::Machine)

    
      2.4  minikube start

    
      2.5  minikube dashboard ( opens up web ui  to access, view and manage kube clusters )



    ![image](https://github.com/user-attachments/assets/68408950-eb80-4676-a4f1-de7c317dc398)



    3.  create a new deployment inside minikube cluster ( file has everything pod creation, replica set creation, using image added in file ) 

         kubectl apply -f f:/deployment.yml


    4. view created deployments
   
       ![image](https://github.com/user-attachments/assets/4358c428-b9fc-4d62-9035-640071823cb9)


      ![image](https://github.com/user-attachments/assets/938c5ba7-96ff-4dca-a688-a9a8666e028c)



    5. delete pod
   
        kubectl delete pod dynamics-5787c64dbf-5tbdm
   
     ![image](https://github.com/user-attachments/assets/9a06060b-c5a3-4dec-ae4c-a699ea429a46)




![image](https://github.com/user-attachments/assets/8da8bbc6-e9ec-4dd0-8878-30df28519a06)



  6. as one pod is deleted the kubelet  will creates new pod as in replica mentioned replicas=1  wenever we delete pod atleast minimun  1 pod will be running in
         the cluster ( minikube )  hence the kubernetes solved auto- healing issue here.


     
     
     

 ![image](https://github.com/user-attachments/assets/28974d86-c60b-4e74-be02-c9b1e9b399fc)


     


