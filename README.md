# Continuous Delivery (CD) pipeline with ArgoCD

We build a Continuous Delivery (CD) pipeline with ArgoCD

We configure the K8s deployment for [Online Boutique](https://github.com/Nicole732/online-boutique) application using ArgoCD. 
This is the CD portion of the CI pipeline found in the App repository.

### Tools
We will use Kustomize to manage environment specific configurations, templating and modularization.

### Use
ArgoCD detects changes in application repository, applies the changes to K8s cluster, and synchronizes the K8s manifests to ensure the cluster is up-to-date. 
ArgoCD handle actual state (in K8s cluster) and desired state (in git repo)  of the K8s cluster, ensures the cluster is always in the desired state as per git repo (only source of truth).

## Benefits 
ArgoCD provides visibility of the changes in K8s cluster through its UI. This configuration enhances the security of EKS cluster by limiting direct access to the cluster and managing deployments through a centralized Git repository.




