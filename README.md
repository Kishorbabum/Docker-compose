# Docker compose with Wordpress and DB 

# Docker-compose
# Docker compose download
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
# Giving permissions for docker-compose
sudo chmod +x /usr/local/bin/docker-compose
# check the docker compose version
docker-compose --version
# Create a wordpress directory
mkdir ~/my_wordpress/
# Change the directory to create a docker-compose.yml file
cd ~/my_wordpress/
# Creating the docker-compose.yml file and get the info of yml file from this repo.
vi docker-compose.yml
# run the docker compose file
docker-compose up -d
# check docker volume ls to know the wordpress and db voulme is created
docker volume ls
# Chcek the docker containers 
docker ps
# check the access of wordpress in browser
<IP>:80 
