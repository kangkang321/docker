FROM centos
RUN curl -Lo /mnt/minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
RUN curl -Lo /mnt/kubectl https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl
RUN curl -Lo /mnt/kubeadm https://storage.googleapis.com/kubernetes-release/release/v1.10.0/bin/linux/amd64/kubeadm
RUN curl -Lo /mnt/kubelet https://storage.googleapis.com/kubernetes-release/release/v1.10.0/bin/linux/amd64/kubelet
RUN curl -Lo /mnt/kubeadm.sha1 https://storage.googleapis.com/kubernetes-release/release/v1.10.0/bin/linux/amd64/kubeadm.sha1
RUN curl -Lo /mnt/kubelet.sha1 https://storage.googleapis.com/kubernetes-release/release/v1.10.0/bin/linux/amd64/kubelet.sha1
RUN curl -Lo /mnt/releases.json https://storage.googleapis.com/minikube/releases.json
