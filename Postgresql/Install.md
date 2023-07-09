## Install Postgresql on kubernetes cluster using ansible playbook ##



![image](https://github.com/sourabhdey21/kubespray/assets/98477908/d5f9d6f1-d44f-482b-bc55-253d5a1a33a4)
As you can see in the below the service has been exposed to port 31818 

Now we can access the postgresql database using the psql cli command

`psql -h 192.168.198.101 -U sourabh --password -p 31818 testDB`


![image](https://github.com/sourabhdey21/kubespray/assets/98477908/05ba47d6-1560-4f2f-8f36-1781500eb8c1)

![image](https://github.com/sourabhdey21/kubespray/assets/98477908/20b0c856-2437-48f4-b79b-957add7d6221)
