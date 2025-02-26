# maven-project
This is a Simple Maven Project created to test maven web application build, Jenkins job creations, docker images build, Kubernetes application deployment.


# Jenkins
After Installing the Jenkins. [ In this project, we are installing the Docker & Ansible in the Jenkins node only ]
. Create a Pipeline
. Pipeline is placed in the file in jenkins/docker-kubernetes-scripted-pipeline.txt file
. Before building the Jenkins Job, there are some pre-requisities.

. Add the Kubernetes node into Known-hosts with the respective user
. Change the kubeconfig path which is placed in the deploy.yaml file.
. Add the Host-key-Checking parameter to false in the ansible.cfg file.
. Add the insecure-registries parameter in the Docker daemon.json file.
. On adding the above parameter, we need to restart docker & Jenkins applications.
. Change the respective IP's, URL's & Credentials used in Jenkins Pipeline job.

