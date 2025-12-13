# SOC stand simulation project

By:
- Galiev Arsen - a.galiev@innopolis.university
- Nguen Ilya-Linh - i.nguen@innopolis.university
- Zavadskii Peter - p.zavadskii@innopolis.university

### Goal/Tasks of the Project

The main goal of the project, is to create a SIEM system following this architecture.

![image](/assets/Architecture.png)

Therefore, we are able not only to prevent different types of vulnarability attacks using firewall (opensource firewall "Suricata") but also manage the system in case of cyber security using Wazuh.

Thus, we have the following stack : 

* 5 virtual machines. 3 Ubuntu, 1 Windows and 1 ParrotOS
* Wazuh (SIEM system)
* Suricata (Firewall)
* Nginx (Load-balancer)

### Configuration plan (Environment preparartion) 

1) Architecture creation, configuring private network using L3 router and starting components deploying.

2) Deploy nginx with custom nginx config that will redirect all the requests to the required servers. Install Suricata firewall and create rules for preventing XSS attacks.

3) Deploy Wazuh master and wazuh agents on different virtual machines and create connection between them. Deloy JuiceShop application to test attacks.


### Development of solution/tests as the PoC 

1) We followed the execution plan and created a private network with all nessecary components.

![image](/assets/development-1.jpg)
---
![image](/assets/development-2.jpg)

### Difficulties faced, new skills acquired during the project

There were several difficulties related to wazuh agent-server connection and Windows machine integration. 


However, we finally coped with it.

![image](/assets/wazuh_master.jpg)

Therefore, we increased our understanding in devops sphere.
### Conclusion, contemplations, and judgment

The project successfully implemented a SOC model based on open tools: Suricata for network protection and Wazuh for Diptych nodes. The architecture with nginx and JuiceShop allows you to test attack detection (for example, XSS) and handle incidents.

The system demonstrated the importance of centralized event collection to quickly identify threats. Such a testbed could become the basis for more complex scenarios, including automation of response (SOAR) and cloud deployment.

## Github link
https://github.com/quintet-sdr/demo-soc
## Demo
