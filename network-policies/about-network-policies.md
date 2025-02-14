Network Policies are a mechanism for controlling network traffic flow in Kubernetes clusters. They allow you to define which of your Pods are allowed to exchange network traffic. You should use them in your clusters to prevent apps from reaching each other over the network, which will help limit the damage if one of your apps is compromised.



There are three different ways to identify target endpoints:

1.Specific Pods (Pods matching a label are allowed)
2.Specific Namespaces (all Pods in the namespace are allowed)
3.IP address blocks (endpoints with an IP address in the block are allowed)
