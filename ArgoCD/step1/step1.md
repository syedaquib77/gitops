
Install Argo CD

```plain
kubectl create namespace argocd

kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
```{{exec}}

After installing Argo CD, wait until the pods are running and ready.

```plain
kubectl get pods -n argocd
```{{exec}}

!!! Help
This guide assumes you have a grounding in the tools that Argo CD is based on. Please read [understanding the basics](https://argo-cd.readthedocs.io/en/stable/understand_the_basics/) to learn about these tools.

If you're stuck then kindly check the Getting Started Page [Argo CD Getting Started](https://argo-cd.readthedocs.io/en/stable/getting_started/)
