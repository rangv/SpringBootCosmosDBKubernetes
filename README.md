![Imported Script](https://github.com/rangv/SpringBootCosmosDBKubernetes/blob/master/images/acskubernetescosmosdb.png "Header Image")
# Deploy Spring Boot CosmosDB App on Azure Container Services (Kubernetes)

#### Software products built around reusable REST based services is very popular and micro service architecture helps in deploying loosely coupled services. Containers make it easy for developers to run their software no matter where it is deployed. Building loosely coupled services by splitting the services based on line of businesses and business functions and deploying them in containers helps in fine grained scalability and versioning. 

#### This article will demostrate deploying a Spring Boot Application on containers using Azure Container Services using Kubernetes orchestrator. App uses CosmosDB as its database. Spring Boot App and CosmosDB are independently scaled. 

![Imported Script](https://github.com/rangv/SpringBootCosmosDBKubernetes/blob/master/images/SpringBootKubernetes.png "Architecture")

#### Azure Container Service for Kubernetes makes it simple to create, configure, and manage a cluster of virtual machines that are preconfigured to run containerized applications. ACS cluster can be created using Azure CLI, PowerShell or Azure portal.

![Imported Script](https://github.com/rangv/SpringBootCosmosDBKubernetes/blob/master/images/SpringbootKubernetescluster.png "Cluster")

![Imported Script](https://github.com/rangv/SpringBootCosmosDBKubernetes/blob/master/images/SpringbootKubernetescluster2.png "Cluster")

#### Master nodes for container orchestration and Worker nodes(Agents) are deployed as VMs. Agents can be scaled in and out using Azure portal, CLI or PowerShell. All nodes are placed in separate subnets with the same virtual network (VNet). A load balancer is placed in front of the master VM, to allow secure shell (ssh). 

![Imported Script](https://github.com/rangv/SpringBootCosmosDBKubernetes/blob/master/images/springbootdocker.png "Docker")

![Imported Script](https://github.com/rangv/SpringBootCosmosDBKubernetes/blob/master/images/springbootdocker2.png "Docker2")

#### Deploy the image to Azure Container Service Kubernetes cluster and expose port for the app to be available over the internet. An external IP is assigned to the app.


![Imported Script](https://github.com/rangv/SpringBootCosmosDBKubernetes/blob/master/images/springbootkubernetesdeploy.png "Deploy")

#### Kebernetes UI is available to manage the cluster and apps. 

![Imported Script](https://github.com/rangv/SpringBootCosmosDBKubernetes/blob/master/images/springbootkuberneteUI.png "UI")

#### Test the deployed App using the external port

![Imported Script](https://github.com/rangv/SpringBootCosmosDBKubernetes/blob/master/images/springbootkubernetetest.png "Test")


#### Monitor with OMS

![Imported Script](https://github.com/rangv/SpringBootCosmosDBKubernetes/blob/master/images/oms-containers-dashboard.png "OMS")


