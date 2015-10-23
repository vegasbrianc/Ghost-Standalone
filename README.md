# Ghost Standalone Docker-Compose Installation
This is a simple docker-compose ghost project that allows you to quickly get up and running with Ghost and volumes mounted to the host so you can store your theme, images, and databases locally.

### Why is this different than the standard Ghost image on the Docker hub? By wrapping Ghost into a Docker compose 

# What you need to do
* Edit the docker-compose.yml with your project information (URL, Host Directory Paths, etc)
* Edit the [config.js](https://github.com/vegasbrianc/Ghost-Standalone/blob/master/ghost/config.js) with your database paths in the database section in both Production and Development sections 
* Edit the [Dockerfile](https://github.com/vegasbrianc/Ghost-Standalone/blob/master/ghost/Dockerfile) with your URL information
