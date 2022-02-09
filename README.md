# my_microk8s

My MicroK8S environment for development
- install microk8s
- enable modules
- set kubectl and helm aliases

# Helms
- mongodb v5 with replicas: 4 replicas, 4GB storage, scripts (install, uninstall, remove PVCs)
- kafka: 2 brokers, 1GB storagee, scripts (install, uninstall, remove PVCs)
- kafka-ui works with Kafka above
- argocd: scripts (install, get password, uninstall)

# Fast exposes
- argocd
- all with kubefwd (https://github.com/txn2/kubefwd/releases)

# Optional exposes (use kubefwd instead)
- mongo
- kafka
- kafka-ui
