# kubernetes
repo is all about kubernetes 


Aim of project :  we will equipped knowledge on kubernetes tech. following topics ive gained skill and exposure 

 cluster ( as master node /control plane ) and 1 worker node is created while creating miniqube installation

 1. install kubectl ( as cli for kubernetes )

   
 3. install minikube

    
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
 

     


