# Project Details 

### What to achieve
1. Deploy React App to the Nginx container and expose to the internet
2. Automate the dployment using ansible
3. All these task should be done in Azure DevOps
4. The containers should run in a VM

Execution steps
1. Created a boilerplate react app
As a requirement I already had npm installed on my machine. 
`npx create-react-app react-docker`
2. Created the Dockerfile and docker-compose.yml
As a requirement I already had npm installed on my machine. 

3. Created an ubuntu machine on Azure via azure cli

4. Created a build pipeline that creates an artifact but does not really build the application code as that would be handle by docker-compose

5. Created a release pipeline and will use the build agent as the ansible agent

6. Copied over the artifacts to the remote ubuntu VM
7. Executed the playbook

*The inventory was placed in variable on azure pipeline to avoid checking in sensitive data in our repository*