# 🤝HIRE US FOR FULL INSTALLATION🤝

Contact Info: archan.fiem.it@gmail.com, hk.sainaga@gmail.com
# Installation Guide(First Phase):
We will install and configure all of the components First and will move to Integrating them one by one.
## Elasticsearch-Kibana:
 - SSH into your VM created for Elastic SIEM
 - Run below commands to spin up elasticseach and kibana using docker. (Note- If any of the below utilities doesn't exists, use "sudo apt install <package>" )
 ```bash
 sudo apt update
 sudo apt upgrade
 sudo apt install docker-compose
 sudo apt install docker.io
 cd /
 wget https://raw.githubusercontent.com/archanchoudhury/SOC-OpenSource/main/codes/elk/docker-compose.yml?token=AMFWN76WO6EJP3LVF5DVHNLBWN7KQ
 sudo docker-compose up -d
 ```
  - Run below to check if the host is listening on 9200, 5601 to confirm the service
 ```bash
 netstat -ltpnd
 ```
  - Now access the Kibana Console from your browser using this- http://Public_IP_ofEc2:5601
 
## TheHive:
  - You can follow the detailed documentation **[HERE](https://docs.thehive-project.org/thehive/installation-and-configuration/installation/step-by-step-guide/)**

## Cortex
 - SSH into the EC2 VM created for Cortex
 - You can follow the detailed documentation **[HERE](https://github.com/TheHive-Project/CortexDocs/blob/master/installation/install-guide.md#elasticsearch-installation)**
  
## MISP
 - You can refer the clear installation Steps [HERE](https://misp.github.io/MISP/INSTALL.ubuntu2004/)
 - For setting up the MISP for first time, watch the tutorial [HERE](https://youtu.be/gSzop2pKM1I)
