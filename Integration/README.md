This is OpenCTI-Wazuh Integration.
In this case I triger OpenCTI feed when match with DNS Server.
When there are request domain to DNS Server, this integrator will try search information about the domain in OpenCTI and send it to Wazuh.

3 parameter need to change:
1. OpenCTI URL
2. OpenCTI API Key
3. GraphQL Query

In my script GraphQL Query specific for *.top domain. I will change it to variable (in progress)
I'll explain more details soon!
