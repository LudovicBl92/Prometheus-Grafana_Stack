
You only need to execute the command: ansible-playbook Run-Prometheus-Grafana.yml.
The playbook Install_Prometheus-Grafana.yml will install Prometheus and in a second time Grafana.
The playbook Configure_Grafana.yml will copy the datasource.yml file in /etc/grafanaprovisioning/datasources. It permit to add your Prometheus server as a datasource.

	  ------------------
	  |   Prometheus   |
	  ------------------

You can log in GUI via http://localhost:9090

	  ------------------ 
	  |    Grafana     |
	  ------------------ 

You can log in GUI via http://localhost:3000
login: admin
password: admin

Then you can go on Configuration tab --> Data sources to see the Prometehus-Server

Finally, go to Dashboard tab --> Manage --> New Dashboard To create your dashboard with the differents metrics as you defined.
