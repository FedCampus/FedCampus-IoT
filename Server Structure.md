# Server Structure

## Base layer
- DKU VCM running ubuntu 22.04 LTS
- Docker CE with Docker compose
## Management layer
- Portainer CE
## Service Layer
### Containers
- **[eclipse-mosquitto](https://hub.docker.com/_/eclipse-mosquitto)** for MQTT Broker
- Database Image TBD
- Server Layer for passing DB calls and accessing different testing parameters
- **[phpmyadmin](https://hub.docker.com/_/phpmyadmin)** for accessing DB for debug purposes
### API for access
- This part is still a work in progress a Nginx Reverse proxy may be deployed for better avaliability and may also allow for easier TLS & authentication
- This part will still be containerlized, but further research is needed
## Todo list
- [ ] Decide on the Database Image to use
- [ ] Provision the VCM
- [ ] Install Docker
- [ ] Install Portainer and setup
- [ ] Develop the service layer
- [ ] Decide on API
