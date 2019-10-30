# ddi-helm-omicsdi
Automation of Omicsdi deployment scripts 

Secrets are needed for deployment's to work 

cd profiledirpath
helm install --name=omicsprofile --namespace=test ./

cd webservicedirpath
helm install --name=omicsservice --namespace=test ./

cd dataflowdirpath
helm install --name=omicsdataflow --namespace=test ./

cd frontenddirpath
helm install --name=omicsfrontend --namespace=test ./
