# Prometheus-Grafana


You only need to execute the command: ansible-playbook Run-Prometheus-Grafana.yml.
The playbook Install_Prometheus-Grafana.yml will install Prometheus and in a second time Grafana.
The playbook Configure_Grafana.yml will copy the datasource.yml file in /etc/grafanaprovisioning/datasources. It permit to add your Prometheus server as a datasource.
The playbook Configure_Prometheus.yml will copy the template prometheus to replace the initial prometheus.yml file to add a new job named grafana 

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

Then you can go on Configuration tab --> Data sources to see the Prometehus-Server.
Next, go to your Prometheus-Server datasource tab and click on dashboard and import Grafana Metrics. 
Finally yuo can see two things on dashboards tabs --> Manage:
	- click on Grafana metrics to see a default panel about Grafana metrics.
	- click on System metrics to see a personnal panel with different dashboard which show you CPU,Memory Usage Available disk, Disk Used and Network Traffic.

