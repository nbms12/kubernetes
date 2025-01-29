# kubernetes
repo is all about kubernetes 


Aim of project :  we will equipped knowledge on kubernetes tech. following topics ive gained skill and exposure 

 cluster ( as master node /control plane ) and 1 worker node is created while creating miniqube installation

 1. install kubectl ( as cli for kubernetes )
 2. install minikube
      2.1 Invoke-WebRequest -OutFile 'c:\minikube\minikube.exe' -Uri 'https://github.com/kubernetes/minikube/releases/latest/download/minikube-windows-amd64.exe' -UseBasicParsing
      2.2  New-Item -Path 'c:\' -Name 'minikube' -ItemType Directory -Force
      2.3  $oldPath = [Environment]::GetEnvironmentVariable('Path', [EnvironmentVariableTarget]::Machine)
             if ($oldPath.Split(';') -inotcontains 'C:\minikube'){
               [Environment]::SetEnvironmentVariable('Path', $('{0};C:\minikube' -f $oldPath), [EnvironmentVariableTarget]::Machine)
      2.4  minikube start
      2.5  minikube dashboard ( opens up web ui  to access, view and manage kube clusters )



    ![image](https://github.com/user-attachments/assets/68408950-eb80-4676-a4f1-de7c317dc398)




