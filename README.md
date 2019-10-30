# ddi-helm-omicsdi
Automation of Omicsdi deployment scripts 

Secrets are needed for deployment's to work, u can ask us to provide secret file

```bash 
cd profiledirpath
helm install --name=omicsprofile --namespace=test ./

cd webservicedirpath
helm install --name=omicsservice --namespace=test ./

cd dataflowdirpath
helm install --name=omicsdataflow --namespace=test ./

cd frontenddirpath
helm install --name=omicsfrontend --namespace=test ./
```

Omicsdi folder for installing Mongodb replica set and Omicsdi web services 

Omicsfront for installing web app and server side rendering

OmicsProfile for installing profile services for user login

spring-cloud-data-flow for installing spring cloud data flow server.

Secret File Required for all deployments :-

apiVersion: v1
kind: Secret
metadata:
  name: omicsdi
type: Opaque
data:
  MONGO_DB: 
  MONGO_USER: 
  MONGO_PASSWD: 
  MONGO_PORT: 
  MONGO_AUTH_DB:
  ORCID_CLIENT_ID: 
  ORCID_CLIENT_SECRET: 
  TOKEN_SECRET: 
  FACEBOOK_APP_KEY: 
  FACEBOOK_APP_SECRET: 
  FACEBOOK_APP_NAMESPACE: 
  GITHUB_CLIENT_ID: 
  GITHUB_CLIENT_SECRET: 
  TWITTER_CONSUMER_KEY: 
  TWITTER_CONSUMER_SECRET: 
  ELIXIR_CLIENT_ID: 
  ELIXIR_CLIENT_SECRET: 
  LINKEDIN_CLIENT_ID: 
  LINKEDIN_CLIENT_SECRET: 
  GOOGLE_CLIENT_ID: 
  GOOGLE_CLIENT_SECRET: 
  DDI_MONGO_MACHINE_ONE: 
  DDI_MONGO_MACHINE_THREE: 
  DDI_MONGO_MACHINE_TWO: 


