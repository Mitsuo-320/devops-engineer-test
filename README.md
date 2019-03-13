# DEVOPS-ENGINEER-TEST

> A fun little technical assessment 

## Prerequisites 
- Azure CLI 
- Python
- Ansible
- Kubectl 
- Minikube (Optional)

## Practical Test
### 1. Kubernetes Cluster
Spin up a Kubernetes cluster on Azure AKS. This can be via the AZ CLI or the Azure dashboard. It can be a single node cluster.

### 2. MongoDB
Deploy a simple MongoDB instance to Kubernetes. It should only be accessible within the cluster.

### 3. Docker
Fork [this repo](https://github.com/rameezk/todo-api-flask) and check-out the code. _Dockerize_ the application. 

Once you're happy, you can push it to the docker registry. Authentication details for the registry will be provided.

Next, create the neccessary Kubernetes resources to serve up this API. Allow the API to be accessible from the internet. 

### 4. Ansible
Create an Ansible playbook to automate the deployment of the API to Kubernetes. You don't have to automate the MongoDB deployment. 

_Dockerize_ the playbook and push it to the Docker registry. This will make the next task easier. 

### 5. GitLab CI
Create a repo on GitLab and push the API repo to it. Create a GitLab CI pipeline for this repo which automatically executes the above playbook on every commit to the _master_ branch. 