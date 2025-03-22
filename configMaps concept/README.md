About configmaps : 

Kubernetes ConfigMap is a built-in Kubernetes API object that’s designed to store your application’s non-sensitive key-value config data.
ConfigMaps allow you to keep config values separate from your code and container images. 
Values can be strings or Base64-encoded binary data.



Once you’ve created a ConfigMap, its content will be saved to your Kubernetes cluster. Pods can then consume the ConfigMap’s values as
environment variables,command line arguments, or filesystem volumes.

Max size of configMap object is 1 MiB

pod3 created . 

![image](https://github.com/user-attachments/assets/04f8d3f5-a3a2-4929-a824-b6b4483367bd)


tested data properties and used in pod3 as an ENV vairable, greetings as variable and values is coming from configmap data. 

![image](https://github.com/user-attachments/assets/c0cc136c-f26d-4599-a013-d6f27ed146ab)
