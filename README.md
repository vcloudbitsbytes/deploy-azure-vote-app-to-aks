# deploy-azure-vote-app-to-aks

This yaml file contains the code that you can copy & paste to deploy containers for running  run some applications.

In this example, we will use sample application called **Azure Vote** provided by Microsoft which is a multi-container application with a web front-end running the sample Azure Vote application and a backend databases using Redis instance in the cluster. 

These containers are available in the Microsoft Container Registry as well.

Two Kubernetes Services are also created:

* An internal service for the Redis instance.
* An external service to access the Azure Vote application from the internet.

## Code
`git clone https://github.com/vcloudbitsbytes/deploy-azure-vote-app-to-aks.git`
`cd configuring-aks`
`kubectl apply -f azure-vote.yml`
`kubectl get service azure-vote-front`
