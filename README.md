#Setup and Configuration:
Created a GitHub repository to host the source code.
Installed Argo CD on my Kubernetes cluster by following the official documentation.
Installed the Argo Rollouts controller in my Kubernetes cluster according to the official guide.

#Creating the GitOps Pipeline:
Dockerized the application by building a Docker image and pushing it to a public container registry.
Modified the Kubernetes manifests in my repository to use the Docker image.
Configured Argo CD to monitor my repository and automatically deploy changes to the Kubernetes cluster.

#Implementing a Canary Release with Argo Rollouts:
Modified the deployment of the application to use Argo Rollouts, specifying a canary release strategy.
Triggered a rollout by making a change to the application, updating the Docker image, and updating the rollout definition.
Monitored the rollout using Argo Rollouts to ensure the canary release completed successfully.
