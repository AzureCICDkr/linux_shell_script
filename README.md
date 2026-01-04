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
chmod +x docker-script/installdocker
sudo docker-script/installdocker

# QEMU
chmod +x etc/installqemu
sudo etc/installqemu

# Kubernetes Control Plane
chmod +x k8s-script/installcontrolplane
sudo k8s-script/installcontrolplane

# Kubernetes Worker Node
chmod +x k8s-script/installworkernode
sudo k8s-script/installworkernode

# Grafana
chmod +x observability-script/grfanascript/installgrafana
sudo observability-script/grfanascript/installgrafana

# Prometheus
chmod +x observability-script/prometheusscript/installprometheus
sudo observability-script/prometheusscript/installprometheus
