# Kustomize, Helm Chart, and ArgoCD

## What is This
Kustomize repository contains jenkins Helm Chart for testing `kustomize` templating. We can later on use the same concept to implement this in `ArgoCD`.

## How to Test
```
$ cd jenkins
$ kustomize build overlays/dev --enable-helm --helm-command helm
```