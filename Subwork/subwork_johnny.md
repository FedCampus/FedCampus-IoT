# subwork\_Johnny
  1. revised docker compose
  2. chose eclipse-mosquitto image as the base of MQTT server
  3. created the github orgnization
  4. Orgnized the file structure of gitbook repo and updated the contents of gitbook page
  5. Installed the [VM Hypervisor](../Server/Server_Provisioning.md)
  6. Requested IP/FQDN from IT
  7. Started on "Server" page of gitbook (need help from [@Jiaqi](https://github.com/luuvy757))
  ### Update March 28th
  - Finished work dividion with Steven He
  - Deployed a working MQTT broker for development
  - Deployed the database for development
  - Implimented remote management
  - Finished persistant IP and FQDN setup on the VMs
  - Rekquested and obtained domain [fedcampus.eu.org](fedcampus.eu.org)
  ### Update April 9th
  - Setted up new mean of remote access
  - Helpdesk framework implimented on [helpdesk](helpdesk.fedcampus.eu.org)
  - Update public key file on ml and iot server
  - Spun up a docker container with access to CUDA at Professor's request
## next step
  1. implement persistance storage (eclipse docs)
  > checked and this part should be implimented on MQTT client side
  2. connect MQTT to Database
  3. setup branch/merge automations for repo

<font color="lightblue">feedback Mar, 16th:
- Learn more knowledge about managing github since we will start to modify code on github this code. 
> Work have started, but current priority for me is to fully setup the server so further development can happen.
- Work on your plan. It's strongly suggested that you should communicate with jinghen before starting write code. Our goal is to implement a basic server with complete functionality within this month.
> Will work on that, initial decision made and will need to work with [@FedML](https://github.com/orgs/FedCampus/teams/fedml)
</font>