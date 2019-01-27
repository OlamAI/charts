## Charts Repository ##
This repository contains all of the Helm charts for deploying services. 

## Deploying and managing services ##
To deploy a service, run  
`helm install --name serviceName ./mychart --set service.type=NodePort`

To override values use the --set flag. More often than not, while developing you will need to override the service type to be a NodePort so it can be accessed externally and tested  
`helm install --name serviceName ./mychart --set service.type=NodePort`

List all currently deployed services  
`helm ls`

Shut down a running service  
`helm del serviceName`