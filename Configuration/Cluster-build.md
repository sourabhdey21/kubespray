# Log in to the ansible node / provision vm

Run following ansible commands to enable IPv4 forwarding and disable swap on all the nodes,

Move to the Kubespary directory

`cd /home/kubesparay/ `

`ansible all -i inventory/mycluster/hosts.yaml -m shell -a "sudo systemctl stop firewalld && sudo systemctl disable firewalld" `

`ansible all -i inventory/mycluster/hosts.yaml -m shell -a "echo 'net.ipv4.ip_forward=1' | sudo tee -a /etc/sysctl.conf" `

`ansible all -i inventory/mycluster/hosts.yaml -m shell -a "sudo sed -i '/ swap / s/^\(.*\)$/#\1/g' /etc/fstab && sudo swapoff -a" `

`ansible-playbook -i inventory/mycluster/hosts.yaml --become --become-user=root cluster.yml `

## Now monitor the deployment, it may take 20 to 30 minutes depending on internet speed and hardware resources.

Once the deployment is completed, we will get following output on our screen,

![image](https://github.com/sourabhdey21/kubespray/assets/98477908/e421b16c-32b9-405c-847b-c2c0ed0bfe9d)


![image](https://github.com/sourabhdey21/kubespray/assets/98477908/d357f5ea-ece2-40f6-abda-c28127cfb243)


![image](https://github.com/sourabhdey21/kubespray/assets/98477908/5f4b1306-c96a-4e3d-baa4-f22d11f863f0)
