This is the OpenCTI-Wazuh Integration.
In this case, I trigger the OpenCTI feed when there's a match on the DNS server.

When a domain request is sent to the DNS server, this integrator searches for information about the domain in OpenCTI and sends the results to Wazuh.

There are three parameters that need to be configured:
1. OpenCTI URL
2. OpenCTI API Key
3. GraphQL Query

In my current script, the GraphQL query is specifically set to search for *.top domains. I’m working on changing that to a variable (still in progress).

For now there is duplication of data from OpenCTI in one json/event, this makes parsing not work properly. I am in the process of working on that 
I will share more details soon!
