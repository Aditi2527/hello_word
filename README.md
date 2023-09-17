# hello_word
### Stable Versions
1. Docker : 1.12.6
2. Kubernetes : 1.7.0
3. NPM : 3.5.2
4. Node Image : Boron

### Tools and Technologies used
1. SCM: Github
2. Build: Shell Script and SSH
3. REPO Management: Docker Hub
4. CI and CD: Jenkins, SSH, and Terraform (K8S cluster creation with Kubernetes Operations via Terraform manifests)
5. Testing: Mocha and SonarQube
6. Collaboration and Communication: Slack
7. Operational Intelligence: Datadog
8. Container Security: Anchore Scanner
9. Deployment: Kubernetes, Amazon Web Services, and Docker
10. Logging: Sematext

## Post Build Actions:
1. Shell Script: Logging into the cluster node. Download the manifests from the Github and apply the changes. Rolling update and rollback options are given through environment variable `DEPLOYMENT_TYPE`. Check `hello-world-ci-cd/post-build.sh`.
2. Setting up the GitHub commit status.
3. Slack Notifications of the build actions to notify the status.

# Highly Available and secure application with Kubernetes, Docker, and AWS.
### Highly Available Kubernetes Cluster on AWS:
1. Node Zones: us-east-1a,us-east-1b,us-east-1c
2. Master Zones: us-east-1a,us-east-1b,us-east-1c
3. Number of Master Nodes: 3
4. Number of Nodes: 3
5. Container Networking: Flannel
6. Cluster Environment: Private
7. Bastion host: Used
8. etc is encrypted for the storage.

### Highly available app with Kubernetes.
App is deployed with Kubernetes deployment and service objects. Check `hello-world-ci-cd/kubernetes/app/`.


