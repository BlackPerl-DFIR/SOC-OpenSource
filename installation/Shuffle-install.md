# 🤝HIRE US FOR FULL INSTALLATION🤝

Contact Info: archan.fiem.it@gmail.com, hk.sainaga@gmail.com
# Shuffle Installation Guide:
  - You can check the full installation guide from [HERE](https://github.com/Shuffle/Shuffle/blob/main/.github/install-guide.html)
  - SSH into the VM which you have spinned up for installing Shuffle
  - Make sure you have [Docker](https://docs.docker.com/get-docker/) and [docker-compose](https://docs.docker.com/compose/install/) installed.
```bash
sudo apt get update
sudo apt upgrade
sudo apt install docker.io
sudo apt install docker-compose
```
  - Download Shuffle
```bash
git clone https://github.com/frikky/Shuffle
cd Shuffle
```
  - Run docker-compose.
```
sudo docker-compose up -d #Wait till the process is completed, shuffle-database folder will now be created.
```
  - Fix prerequisites for the Opensearch database (Elasticsearch):
```bash
sudo chown 1000:1000 -R shuffle-database 		
```
  - Restart docker-compose.
```
sudo docker-compose restart
```
  - Once done verify your service by checking below
```bash
sudo docker ps
sudo docker logs <container-id> follow
```
  - From your browser access- https://Public-IP:3443
