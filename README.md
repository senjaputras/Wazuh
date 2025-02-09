# Wazuh-Archivers
How to collect raw log / all log (logall) using Wazuh.

What is Raw Log? <br>
Not only match with Rules only will index on Wazuh, but also log that doesnt match with rules.

You only need to edit <b>ossec.conf</b> in *WAZUH-MANAGER*. <br>
It will make Wazuh-Manager to store all log that shipping by wazuh-agent to file. 
