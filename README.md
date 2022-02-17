# @BCsabaEngine microk8s developer environment

My MicroK8S environment with helm for development
- install microk8s
- enable modules: dns, storage, registry
- install: helm(3), dashboard
- init kube config
- set kubectl and helm aliases
- add needed helm repos

# Start-Stop microk8s
- 0.start_k8s at morning
- 1.reinit if your local IP changed (because move from home to office)
- 9.stop_k8s after worktime

# Helms - install if needed
- mongodb v5 with replicas: 2 replicas, 4Gi storage, 2Gi memory, scripts (install, uninstall, remove PVCs)
- kafka: 2 brokers, 1Gi storagee, 512Mi memory, scripts (install, uninstall, remove PVCs)
- kafka-ui works with Kafka above
- elastic: default settings [huge RAM needed] scripts (install, uninstall, remove PVCs)
- argocd: scripts (install, get password, uninstall)

# Fast exposes - run after start
- argocd
- k8s dashboard
- all with kubefwd (https://github.com/txn2/kubefwd/releases)
- use with https://app.elasticvue.com/ or same Chrome plugin

# Optional exposes (use kubefwd instead)
- mongo
- kafka
- kafka-ui
- elastic
