# Kustomize Demo

### Install k3s
```
 $ curl -sfL https://get.k3s.io | sh - 
 # Check for Ready node, takes ~30 seconds 
 $ k3s kubectl get node 
```

### Install kustomize CLI
```
 $ snap install kustomize 
```

### Build the manifests

```
kustomize build overlays/prod/|kubectl apply -f -
```

