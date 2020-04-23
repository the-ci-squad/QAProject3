# QAProject3
**presentation link: https://docs.google.com/presentation/d/1gGrvONwapNHR8NOhoLwujwI5iRfyucv5LorXDcGmSqM/edit?usp=sharing**


## Contents 
* [Introduction](#Introduction) -*Project Brief, Intended Solution*
* [CI/CD Pipeline](#dep_pipeline) -*Description, Pipeline*
* [Planning](#planning) -*Plans, Members, Roles, Decision-Making*
* [Use Cases](#UserCases)
* [Risk Analysis](#Risk) 
* [Technologies Used](#Technology)-*Ansible, Azure, Git, Jenkins, Kubernetes, Terraform, Nginx* 
* [Testing](#Testing)
* [Deployment](#Deployment)
* [Costs](#Costs) 
* [Project Conclusion](#Conclusion) 
* [Future Work](#FutureWork) 


<a name="Introduction"></a>
## Introduction 
#### *Project Brief*
The brief for this project was to plan, design and implement a solution for automating the deployments and development workflows of the following projects:
 
**Frontend client** https://github.com/spring-petclinic/spring-petclinic-angular

**Backend API** https://github.com/spring-petclinic/spring-petclinic-rest

More info on the Source Code: https://projects.spring.io/spring-petclinic/
 
 
#### *Intended Solution*
As a team we decided the direction of our part of the project would utilise technologies that we were either familiar with or had related knowledge that could be transferable to a different technology. We intended to create multiple environments for development, for deployment and load balancing whilst follwoing our planned pipeline. 

The creating would be handled using Ansible, Terraform and Kubernetes. The deployment aspect of this is intended to have automated build and redeployment based on any change made to the respective github repositories for the backend and frontend and handled with Jenkins. The load balancing for incoming traffic would be handled with Nginx, whilst costs would be tracked through the Azure Cost Tracking Utility Tool.

<a name="dep_pipeline"></a>
## CI/CD Pipeline
#### *Description*
The pipeline structure we decided upon made use of Version control system Git with repositories hosted by Github, this is where all files relevant to the project will be stored on relevant branches.

Terraform is being used to actively create the Virtual Machines through the Azure CLI, then Ansible is being applied to create and set up the environments, Git is then used to pull relevant files to their intended environments, once the source code is editted and pushed (uploaded) to Git this will invoke Jenkins to build, test and deploy the product using Kubernetes. 

#### *Pipeline*

![](https://github.com/the-ci-squad/QAProject3/blob/tino_terraform_ansible/README_FILES/INITAL-CI-PIPELINE-DESIGN.jpg)


<a name="planning"></a>
## Planning
*Plans, Members, Roles, Decision-Making*
#### *Plans*
As this project has such large goal with a sample amount of time and no communication with developers it was important to have adequate planning, internal communication methods and project management in place. For this we decided that we would have 1 a daily Scrum and subsequent meetings when necessary. The scrums were used largely for most of the planning but unlike traditional planning meetings scrums core values are to instill courage, focus, respect, openness and commitment in relation to a project and its team. To track our plan we used Trello, an online, Kanban-style, list-making application, to keep track of progress, any issues and completed tasks. To communicate we utilised Microsoft Teams as it was convenient and had screen sharing capablities which would help with troubleshooting team members' issues.  

A link for further information about Scrums, Teams and Trello
https://www.scrum.org/resources/what-is-scrum

https://www.microsoft.com/en-gb/microsoft-365/microsoft-teams/group-chat-software

https://help.trello.com/article/708-what-is-trello

#### *Team members*
Tino - https://github.com/tinokingstone

Benjie - https://github.com/BenjieA

Stef - https://github.com/stefangelova

Harman - https://github.com/hman191



#### *Roles/Tasks:* 
Stef - Kubernetes/Docker

Tino - Terraform/Ansible/Docker

Benjie - Jenkins/Ansible/Docker

Harman - SQL/General Assistance/Docker

#### *Scrum Master* 
Harman

#### *Decision-Making*
During the decision making process was driven by Trainer Jay Grindrod acting as the Product Owner and listening in on Scrums and certain meeting that would coincide with the Product Owners interests. Within the team any major decisons would be discussed and the approach would be decided based on which option was deemed most logical. These approaches would then be added to the Trello/planning board in order to keep track of the progress being made.




<a name="UserCases"></a>
## User Stories


<a name="Risk"></a>
## Risk Assessment

<a name="Technology"></a>
## Technologies Used

*Trello
*Ansible
*Terraform
*Azure
*Jenkins
*Kubernetes
*Docker
*Nginx

<a name="Testing"></a>
## Testing

<a name="Deployment"></a>
## Deployment

<a name="Costs"></a>
## Costs 

<a name="Conclusion"></a>
## Project Conclusion

