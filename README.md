```text
Architecture
------------
linux_shell_script
├── docker-script
│   └── installdocker
├── etc
│   └── installqemu
├── k8s-script
│   ├── installcontrolplane
│   └── installworkernode
└── observability-script
    ├── grfanascript
    │   └── installgrafana
    └── prometheusscript


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
