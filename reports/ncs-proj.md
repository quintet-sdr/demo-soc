# SOC stand simulation project

By:
- Galiev Arsen - a.galiev@innopolis.university
- Nguen Ilya-Linh - i.nguen@innopolis.university
- Zavadskii Peter - p.zavadskii@innopolis.university

### Goal/Tasks of the Project 

The main goal of the project, is to create a SIEM system following this architecture.

![image](/assets/Architecture.png)

Therefore, we are able not only to prevent different types of vulnarability attacks using firewall (opensource firewall "Suricata") but also manage the system in case of cyber security using Wazuh.

### Execution plan/Methodology

1) Architecture creation, configuring private network using L3 router and starting components deploying.

2) Deploy nginx with custom nginx config that will redirect all the requests to the required servers. Install Suricata firewall and create rules for preventing XSS attacks.

3) Deploy Wazuh master and wazuh agents on different virtual machines and create connection between them. Deloy JuiceShop application to test attacks.


### Development of solution/tests as the PoC 

1) We followed the execution plan and created a private network with all nessecary components.

### Difficulties faced, new skills acquired during the project

### Conclusion, contemplations, and judgment