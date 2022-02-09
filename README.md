# my_microk8s

My MicroK8S environment with helm for development
- install microk8s
- enable modules
- init kube config
- set kubectl and helm aliases
- add needed helm repos

# Start-Stop microk8s
- 1.start_k8s at morning
- 9.stop_k8s after worktime

# Helms - install if needed
- mongodb v5 with replicas: 4 replicas, 4GB storage, scripts (install, uninstall, remove PVCs)
- kafka: 2 brokers, 1GB storagee, scripts (install, uninstall, remove PVCs)
- kafka-ui works with Kafka above
- argocd: scripts (install, get password, uninstall)

# Fast exposes - run after start
- argocd
- k8s dashboard
- all with kubefwd (https://github.com/txn2/kubefwd/releases)

# Optional exposes (use kubefwd instead)
- mongo
- kafka
- kafka-ui
