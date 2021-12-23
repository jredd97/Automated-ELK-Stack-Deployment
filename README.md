# Automated-ELK-Stack-Deployment
The files in this repository were used to configure the network depicted below.
## Automated ELK Stack Deployment

The files in this repository were used to configure the network depicted below.

![Network Diagram](https://github.com/CJBOULDER/CyberSecurityBootcamp/blob/main/Diagrams/Network_Design.png "Network Diagram")

These files have been tested and used to generate a live ELK deployment on Azure. They can be used to either recreate the entire deployment pictured above. Alternatively, select portions of the _____ file may be used to install only certain pieces of it, such as Filebeat.

! [ansible.cfg] (https://github.com/jredd97/Automated-ELK-Stack-Deployment/blob/main/Ansible/ansible.cfg)
! [hosts] (https://github.com/jredd97/Automated-ELK-Stack-Deployment/blob/main/Ansible/hosts)
! [install-elk.yml] (https://github.com/jredd97/Automated-ELK-Stack-Deployment/blob/main/Ansible/install-elk.yml)
! [filebeat-config.yml] (https://github.com/jredd97/Automated-ELK-Stack-Deployment/blob/main/Ansible/filebeat-config.yml)
! [filebeat-playbook.yml] (https://github.com/jredd97/Automated-ELK-Stack-Deployment/blob/main/Ansible/filebeat-playbook.yml)
! [metricbeat-config.yml] (https://github.com/jredd97/Automated-ELK-Stack-Deployment/blob/main/Ansible/metricbeat-config.yml)
! [metricbeat-playbook.yml] (https://github.com/jredd97/Automated-ELK-Stack-Deployment/blob/main/Ansible/metricbeat-playbook.yml)


This document contains the following details:
- Description of the Topology
- Access Policies
- ELK Configuration
  - Beats in Use
  - Machines Being Monitored
- How to Use the Ansible Build


### Description of the Topology

The main purpose of this network is to expose a load-balanced and monitored instance of DVWA, the D*mn Vulnerable Web Application.

Load balancing ensures that the application will be highly efficient, in addition to restricting in-bound access to the network.

What aspect of security do load balancers protect?
Load Balancing plays an important security role as computing moves evermore to the cloud. The off-loading function of a load balancer defends an organization against distributed denial-of-service (DDoS) attacks. It does this by shifting attack traffic from the corporate server to a public cloud provider.
What is the advantage of a jump box?
 Load balancing lets you evenly distribute network traffic to prevent failure caused by overloading a particular resource. This strategy improves the performance and availability of applications, websites, databases, and other computing resources. It also helps process user requests quickly and accurately.


Integrating an ELK server allows users to easily monitor the vulnerable VMs for changes to the data and system logs.
What does Filebeat watch for?
Installed as an agent on your servers, Filebeat monitors the log files or locations that you specify, collects log events, and forwards them.
	
What does Metricbeat record?
Metricbeat helps you monitor your servers by collecting metrics from the system and services running on the server.

The configuration details of each machine may be found below.

| Name       | Function                                                                | IP Address | Operating System |
|---------------|-----------------------------------------------------------------|-----------------|------------------|
| Jump Box | Gateway                                                               | 10.0.0.4      | Linux Ubuntu Pro 18.04 |
| Web-1       | Host for container running DVWA                        | 10.0.0.5      | Linux Ubuntu Pro 18.04 |
| Web-2       | Host for container running DVWA                         |  10.0.0.6    | Linux Ubuntu Pro 18.04 |
| Elk-Server | Monitoring and log aggregation for DVWA hosts  |10.1.0.10    | Linux Ubuntu Pro 18.04 |
