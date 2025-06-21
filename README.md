# K8s minikube cluser setup

1. Install kubectl (https://kubernetes.io/docs/tasks/tools/)
2. Install VirtualBox (https://www.virtualbox.org/wiki/Downloads)
    - sudo apt-get update
    - sudo apt-get install virtualbox
3. minikube documentation (https://minikube.sigs.k8s.io/docs/)
    - Installation (https://minikube.sigs.k8s.io/docs/start/?arch=%2Flinux%2Fx86-64%2Fstable%2Fdebian+package)
4. Start minikube with virtualbox - minikube start -driver=virtualbox
    - Check in VirtualBox Manager application to check the VM status
    - minikube command to check the status - minkube status
    - List available add-ons - minikube addons list
5. Stop minikube - minikube stop
6. Delete minikube cluster - minikube delete