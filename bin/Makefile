all: helm kubectl kubeseal kustomize octant


helm:
	curl -L -O https://get.helm.sh/helm-v3.5.2-linux-amd64.tar.gz
	tar zxvf ./helm-v3.5.2-linux-amd64.tar.gz linux-amd64/helm \
		--to-stdout > ./helm
	chmod 775 ./helm
	rm helm-v3.5.2-linux-amd64.tar.gz


kubectl:
	curl -L https://dl.k8s.io/release/v1.21.0/bin/linux/amd64/kubectl \
		> ./kubectl
	chmod 775 ./kubectl


kubeseal:
	curl -L https://github.com/bitnami-labs/sealed-secrets/releases/download/v0.15.0/kubeseal-linux-amd64 \
		> ./kubeseal
	chmod 775 ./kubeseal


kustomize:
	curl -L -O https://github.com/kubernetes-sigs/kustomize/releases/download/kustomize%2Fv3.8.1/kustomize_v3.8.1_linux_amd64.tar.gz
	tar zxvf kustomize_v3.8.1_linux_amd64.tar.gz kustomize \
		--to-stdout > ./kustomize
	chmod 775 ./kustomize
	rm kustomize_v3.8.1_linux_amd64.tar.gz


octant:
	curl -L -O https://github.com/vmware-tanzu/octant/releases/download/v0.20.0/octant_0.20.0_Linux-64bit.tar.gz
	tar zxvf ./octant_0.20.0_Linux-64bit.tar.gz octant_0.20.0_Linux-64bit/octant \
		--to-stdout > ./octant
	chmod 775 ./octant
	rm octant_0.20.0_Linux-64bit.tar.gz
