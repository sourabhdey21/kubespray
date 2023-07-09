# Additional Changes in Ansible node for making the cluster 


`cd /home/kubespary`

` declare -a IPS=(192.168.198.100 192.168.198.100 192.168.198.101 192.168.198.102 192.168.198.103 192.168.198.104)`

`CONFIG_FILE=inventory/mycluster/hosts.yaml python3 contrib/inventory_builder/inventory.py ${IPS[@]}`

# Validate the Configuration File 

`cat inventory/mycluster/hosts.yaml`

 ![image](https://github.com/sourabhdey21/kubespray/assets/98477908/67305117-0dd8-4c00-8f55-6378725b3495) 


# Add this parameter in cluster.yaml

`vi inventory/mycluster/group_vars/k8s_cluster/addons.yml`


dashboard_enabled: true

ingress_nginx_enabled: true

ingress_nginx_host_network: true

![image](https://github.com/sourabhdey21/kubespray/assets/98477908/0e7add0e-3753-47a4-a451-4152286e8d6e)

