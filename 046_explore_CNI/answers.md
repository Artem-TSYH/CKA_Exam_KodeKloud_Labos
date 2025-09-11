## Linux-Commands: ##

* ps
* ps aux

### 1/5. Inspect the kubelet service and identify the container runtime endpoint value is set for Kubernetes. ###

ps aux | grep endpoint  
ps aux | grep -i kubelet

### 2/5. What is the path configured with all binaries of CNI supported plugins? ###

Documentation:  
https://kubernetes.io/docs/concepts/extend-kubernetes/compute-storage-net/network-plugins/

### 3/5. Identify which of the below plugins is not available in the list of available CNI plugins on this host? ### 

Check the list in the directory:  
cd /opt/cni/bin  
(see Documentation above)  

### 4/5. What is the CNI plugin configured to be used on this kubernetes cluster? ###

Check the list in the directory:  
cd /etc/cni/net.d  
(see Documentation above)  
  
kubectl get daemonset -n kube-system  

### 5/5. What binary executable file will be run by kubelet after a container and its associated namespace are created? ###

Check the list in the directory:  
cd /etc/cni/net.d  
(see Documentation above)  