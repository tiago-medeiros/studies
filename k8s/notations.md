# Kubernetes studies notations

## Learn and practice imperative commands
- Remember to use **run** or **create** parameters with **--dry-run=client** and **-o yaml** to generate yaml files when is necessery to edit some inputs

### Taints Tolerations and Node Affinity
To make sure that a specific node (like one with GPU or ARM processor) will only host an specific kind of pod it is necessery to apply taint/tolerations to avoid other pods to run those nodes and node affinity to garante that the desire pods will be allocate on right node

### Requests and Limits

- LimitRange
Set the default values for request and limits for pods creates without it
It will applicable at the namespace level
This only affect pods created after the limit range is created or update

- Resource Quotas


### Static PODs
The default path is /etc/kubernetes/manifests but it can be modified
check the file /var/lib/kubelet/config.yaml to know where static will be loaded
