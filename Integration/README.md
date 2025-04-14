This is the OpenCTI-Wazuh Integration.
In this case, I trigger the OpenCTI feed when there's a match on the DNS server.

When a domain request is sent to the DNS server, this integrator searches for information about the domain in OpenCTI and sends the results to Wazuh.

There are three parameters that need to be configured:

OpenCTI URL

OpenCTI API Key

GraphQL Query

In my current script, the GraphQL query is specifically set to search for *.top domains. I’m working on changing that to a variable (still in progress).

I’ll share more details soon!
