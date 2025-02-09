# Wazuh-Archivers
How to collect raw log / all log (logall) using Wazuh.

What is Raw Log? <br>
Not only match with Rules only will index on Wazuh, but also log that doesnt match with rules.

1. You only need to edit **ossec.conf** in *WAZUH-MANAGER*. <br>
    It will make Wazuh-Manager to store all log that shipping by wazuh-agent to file. 

    In ossec.conf edit this line.
    
        <logall>no</logall>
        <logall_json>no</logall_json>
    
   Change **No** value to **Yes**. <br>
   If configuration works, in Wazuh-Manager check log at /var/ossec/logs/archives/ it should generate *.json.log.

2. Access raw-log using GUI (Wazuh-dashboard / Kibana).
   Go to filebeat configuration **filebeat.yml** at /etc/filebeat/
   Go to this line.
   
        filebeat.modules:
        - module: wazuh
          alerts:
            enabled: true
          archives:
            enabled: no
    
   Change **archives** to **true**

3. Last, create index pattern **wazuh-archives-*** on Wazuh-dashboard/kibana
