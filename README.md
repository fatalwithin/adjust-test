# adjust-test

## Initial task

Scenario  
  
A web app running on port 80 needs to be deployed to a Kubernetes install. For the sake of
this test, please tailor your answer to use a local instance of minikube.  
You are tasked with automating the deployment process pipeline, to containerize and deploy
the application to Kubernetes.
Please use the sample Ruby application https://github.com/sawasy/http_server.
It runs on TCP port 80. The application also exposes a health check and endpoint at the route
/healthcheck.  
  
You can use any infrastructure as code tools to package, deploy and run the application. For
example: Ansible, Terraform, K8s, etc.  
Please make sure you commit each step of your progress with descriptive commits so we can
follow up with the development of the project.  

You are tasked with automating the deployment process pipeline, to containerize and deploy
the application to Kubernetes.  

Requirements  
  
Please ensure your submission includes all of the following.  
- Highly available and load balanced environment is required  
- Docker is the tool to support it  
- Ensuring the application is started before served with traffic  
- Enhancing availability with probes  
- Running application as non-root  
- A README with:  
  - step-by-step instructions to recreate the setup  
  - the Strategy/Architecture  
  - Instructions on how to connect to the running application  
- All the scripts, configs, playbooks, manifest etc should be provided on a DVCs, preferably Github.  
- If your test requires a non-current version of software, please explain why.  
    
## Solution

