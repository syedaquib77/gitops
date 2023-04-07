
Install Argo CD using Non-HA manifests in argocd namespace.

use these manifests: `/tmp/install.yaml`

After installing Argo CD, make sure that pods are running and ready.

<br>
<details><summary>Solution</summary>
<br>

```plain
kubectl create namespace argocd

kubectl apply -n argocd -f /tmp/install.yaml
```{{exec}}

Wait until the pods are running and ready

```plain
kubectl get pods -n argocd
```{{exec}}

</details>
