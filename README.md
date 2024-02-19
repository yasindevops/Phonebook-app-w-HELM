# Project-206: Microservice Architecture for Phonebook Web Application using Kubernetes (HELM Package)

This project aims to deploy a Microservice Architecture-based Phonebook Web Application using Python Flask, Docker and Kubernetes. The project includes a backend service for CRUD (Create/Read/Update/Delete) operations, a separate service for search operations, and a MySQL database.

# Installation

## Setup Kubernetes Environment:

- Create your Kubernetes environment using the CloudFormation template,
- Check your Kubernetes environment using the kubectl command.

```
kubectl get nodes
kubectl get pods -o wide
```

## Download and Install HELM Package:

- Copy the GitHub repo link and navigate to a local directory,
- Download and install the HELM package.

```
git clone [GitHub_Repo_Link]
cd [Project_Folder]
helm install [Release_Name] 
```

## Using the Application:

Once the installation is complete, you can access the application at the following addresses:

```
http://[EC2_Public_IP]:30001/ - CRUD Operations
http://[EC2_Public_IP]:30002/ - Search Operation
```

### Notes:

- Sensitive information such as database connection passwords is securely managed using Kubernetes secrets and configMap features.
- The MySQL database is stored on a Persistent Volume Claim (PVC) for the application to function.
- The application is containerized using Docker and Kubernetes, making it easily deployable with the HELM package.

### Development:

- To contribute to the project, follow the GitHub repo link and submit pull requests.
- This README file provides basic information to help users install and use your project. You can add more specific details and development instructions as needed for your project.
