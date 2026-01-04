```text
Architecture
------------
linux_shell_script
├── db
│   ├── docker-compose.yaml
│   ├── initdb
│   │   └── init-db.sql
│   ├── install_mysql
│   └── remove_mysql
│
├── devops-script
│   ├── devops_vm_script
│   └── docker-compose.yaml
│
├── docker-script
│   ├── docker.asc
│   └── install_docker
│
├── etc
│   ├── install_gitea
│   ├── install_qemu
│   └── setup_git_gitea_binary
│
├── k8s-script
│   ├── install_control_plane
│   ├── install_remote_kubectl
│   ├── install_upgrade_test_control_plane
│   ├── install_upgrade_test_node
│   ├── install_worker_node
│   └── resetk8snode
│
├── nats-script
│   └── install_nats
│
├── nexus-script
│   ├── install_nexus
│   └── remove_nexus
│
├── observability-script
│   ├── grafana-script
│   │   └── install_grafana
│   │
│   └── prometheus-script
│       ├── common-script
│       │   ├── install_alert_manager
│       │   ├── install_blackbox_exporter
│       │   ├── install_mysql_exporter
│       │   └── install_node_exporter
│       │
│       ├── install_prometheus
│       └── remove_prometheus
│
└── redis-script
    └── install_redis



Execution
---------

# Docker
chmod +x docker-script/install_docker
sudo ./docker-script/install_docker

# QEMU
chmod +x etc/install_qemu
sudo ./etc/install_qemu

# Kubernetes Control Plane
chmod +x k8s-script/install_control_plane
sudo ./k8s-script/install_control_plane

# Kubernetes Worker Node
chmod +x k8s-script/install_worker_node
sudo ./k8s-script/install_worker_node

# Kubernetes Remote Kubectl
chmod +x k8s-script/install_remote_kubectl
sudo ./k8s-script/install_remote_kubectl

# Kubernetes Upgrade Test Control Plane
chmod +x k8s-script/install_upgrade_test_control_plane
sudo ./k8s-script/install_upgrade_test_control_plane

# Kubernetes Upgrade Test Node
chmod +x k8s-script/install_upgrade_test_node
sudo ./k8s-script/install_upgrade_test_node

# Reset Kubernetes Node
chmod +x k8s-script/resetk8snode
sudo ./k8s-script/resetk8snode

# MySQL Install
chmod +x db/install_mysql
sudo ./db/install_mysql

# MySQL Remove
chmod +x db/remove_mysql
sudo ./db/remove_mysql

# NATS
chmod +x nats-script/install_nats
sudo ./nats-script/install_nats

# Nexus Install
chmod +x nexus-script/install_nexus
sudo ./nexus-script/install_nexus

# Nexus Remove
chmod +x nexus-script/remove_nexus
sudo ./nexus-script/remove_nexus

# Grafana
chmod +x observability-script/grafana-script/install_grafana
sudo ./observability-script/grafana-script/install_grafana

# Prometheus
chmod +x observability-script/prometheus-script/install_prometheus
sudo ./observability-script/prometheus-script/install_prometheus

# Alert Manager
chmod +x observability-script/prometheus-script/common-script/install_alert_manager
sudo ./observability-script/prometheus-script/common-script/install_alert_manager

# Blackbox Exporter
chmod +x observability-script/prometheus-script/common-script/install_blackbox_exporter
sudo ./observability-script/prometheus-script/common-script/install_blackbox_exporter

# MySQL Exporter
chmod +x observability-script/prometheus-script/common-script/install_mysql_exporter
sudo ./observability-script/prometheus-script/common-script/install_mysql_exporter

# Node Exporter
chmod +x observability-script/prometheus-script/common-script/install_node_exporter
sudo ./observability-script/prometheus-script/common-script/install_node_exporter

# Redis
chmod +x redis-script/install_redis
sudo ./redis-script/install_redis

# Gitea
chmod +x etc/install_gitea
sudo ./etc/install_gitea

# DevOps VM Script
chmod +x devops-script/devops_vm_script
sudo ./devops-script/devops_vm_script

