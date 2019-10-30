# ddi-helm-omicsdi
Automation of Omicsdi deployment scripts 

Secrets are needed for deployment's to work, u can ask us to provide secret file

cd profiledirpath
helm install --name=omicsprofile --namespace=test ./

cd webservicedirpath
helm install --name=omicsservice --namespace=test ./

cd dataflowdirpath
helm install --name=omicsdataflow --namespace=test ./

cd frontenddirpath
helm install --name=omicsfrontend --namespace=test ./

Omicsdi folder for installing Mongodb replica set and Omicsdi web services 

Omicsfront for installing web app and server side rendering

OmicsProfile for installing profile services for user login

spring-cloud-data-flow for installing spring cloud data flow server.


