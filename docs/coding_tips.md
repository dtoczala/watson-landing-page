# IBM Watson - Coding Tips and Tricks

This content is changing over time.  Please clean up anything that is out of date.  

## Good General Watson Architecture Practices
### Have a Secondary Watson service Instance
It is good architectural practice to have a second Watson service instance for your Watson services, and that it be located in a different Kubernetes cluster, and a different data center.  This gives you the ability to gracefuly degrade should you lose connectivity to, or the service of, one of your Watson service instances.
_Note: You should not have to do this in development environments.  You can test failover capability in test and performance environments prior to deployment.

## Good General Watson Coding Practices
### Use Environmental Parameters for Watson service endpoints
It is good coding practice to use two environmental parameters in your code.  One for a primary Watson service endpoint, and one for your secondary (or failover) Watson service endpoint.  So if you had a colaboration layer application that communicated with Watson Assistant, you would have the following:
- One called PRIMARY_WA_ENDPOINT
- One called SECONDARY_WA_ENDPOINT
