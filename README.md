# Kubernetes Setup

# Install ArgoCD

```bash
git clone git@github.com:estevaofay/argocd.git
cd argocd
kubectl apply --kustomize argocd-setup
```

# Add access to private repo
```bash
argocd repo add git@github.com:estevaofay/argocd.git --ssh-private-key-path ~/.ssh/id_ecdsa
```
# Install bootstrap

```bash
kubectl apply --kustomize bootstrap
```
