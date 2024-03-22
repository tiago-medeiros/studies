# Releases

Vmajor.minor.path


## Core controle plane components 
- kube-apiserver
- Controller-manager
- kube-scheduler
- kubelet
- kube-proxy

None of the other componentes should ever be in higher version than the kube-apiserver.
The controller-manager and kube-scheduler can be one version lower than the kube-apiserver. kubelet and kube-proxy can be 2 versions lower than the kube-api-server. 
If kube-apiserver was in the version v1.10, then the controller-manager and kube-scheduler can be at 1.9 or v1.10.
kubelet and kube-proxy can be at 1.8, 1.9 or 1.10

The recomended is to upgrade one version at the time. e.g 1.10 to 1.11 then to 1.12...
