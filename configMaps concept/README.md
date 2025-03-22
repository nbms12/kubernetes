About configmaps : 

Kubernetes ConfigMap is a built-in Kubernetes API object that’s designed to store your application’s non-sensitive key-value config data.
ConfigMaps allow you to keep config values separate from your code and container images. 
Values can be strings or Base64-encoded binary data.



Once you’ve created a ConfigMap, its content will be saved to your Kubernetes cluster. Pods can then consume the ConfigMap’s values as
environment variables,command line arguments, or filesystem volumes.

Max size of configMap object is 1 MiB


