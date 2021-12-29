# 🤝HIRE US FOR FULL INSTALLATION🤝

Contact Info: archan.fiem.it@gmail.com, hk.sainaga@gmail.com
# Beat Agent Installation Guide:
  - You can follow the installation guide [HERE](https://www.elastic.co/guide/en/beats/filebeat/current/filebeat-installation-configuration.html)
  - Below are the details steps involved
```bash
curl -L -O https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-7.X.X-amd64.deb
sudo dpkg -i filebeat-7.X.X-amd64.deb
```
  - Change the filebeat config files at /etc/filebeat/filebeat.yml
  - Start the filebeat service
```bash
sudo system start filebeat
```
  - Now check your Kibana Console under filebeat* index
