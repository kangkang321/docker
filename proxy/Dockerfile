FROM centos
RUN curl -Lo /mnt/minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
RUN curl -Lo /mnt/kubectl https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl
RUN curl -Lo /mnt/kubeadm http://storage.googleapis.com/kubernetes-release/release/v1.10.0/bin/linux/amd64/kubeadm
RUN curl -Lo /mnt/kubelet http://storage.googleapis.com/kubernetes-release/release/v1.10.0/bin/linux/amd64/kubelet


