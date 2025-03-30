Sometimes documentation or tutorial in internet skip important small step.

This is my Wazuh explorer.

First of all. In this documentation I use **Centralized Configuration**. Where agent can be configured remotely by using the agent.conf.
In this directory there is file "agent.conf". That file include all of configuration wazuh-agent capability: 
- Vulnerability Detection
- FIM (File Integrity Monitoring)
- System Inventory
- SCA (Security Configuration Assessment)

There are 2 way to configure wazuh-agent:
1. Local Configuration (ossec.conf)
2. Centralized Configuration (agent.conf)
