all:
	helm -n monitoring template \
		prometheus prometheus-community/kube-prometheus-stack \
		--version 14.0.1 \
		--set alertmanager.ingress.enabled=True \
		--set alertmanager.ingress.hosts='{alertmanager.local}' \
		--set alertmanager.ingress.ingressClassName=nginx \
		--set grafana.ingress.enabled=True \
		--set grafana.ingress.hosts='{grafana.local}' \
		--set grafana.ingress.ingressClassName=nginx \
		--set prometheus.ingress.enabled=True \
		--set prometheus.ingress.hosts='{prometheus.local}' \
		--set prometheus.ingress.ingressClassName=nginx \
		> template.yaml
