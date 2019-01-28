# ADSK

Ansible configuration with stats storage and stats gathering.

##Components
* Nginx with load balancer and proxy pass configuration
* Ansible automation
* Telegraf, InfluxDB and Grafana with fully featured dashboard
* Systemd service to run Java (Spring) application


## Project visualisation
![visualisation](https://github.com/duudey/ADSK_final/blob/master/Przechwytywanie.PNG)
## How to use 

1. Prepare machines for hosts groups:
* one server for nginx reversed proxy and letsencrypt
* one servers for running application
* server for gathering and presenting stats (metrics)
2. set variables values in server.ini and infrastructure.yml
3. use ssh-agent and add id_student 
3. run `ansible-playbook -i servers.ini infrastructure.yml`

## Addition information
Grafana for now don't have dashboards
There in future will be added second application server
