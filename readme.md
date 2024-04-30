# Kustomize, Helm Chart, and ArgoCD

## What is This
Kustomize repository contains jenkins Helm Chart for testing `kustomize` templating. We can later on use the same concept to implement this in `ArgoCD`.

## How to Test for Jenkins
```
$ cd kustomize/jenkins
$ kustomize build overlays/dev --enable-helm 
```

## How to Implement for Jenkins
```
$ cd kustomize/jenkins
$ kustomize build overlays/dev --enable-helm | oc apply -f
```

## How to Test for Sonarqube
```
$ cd kustomize/sonarqube
$ kustomize build overlays/dev --enable-helm 
```

## How to Implement for Sonarqube
```
$ cd kustomize/sonarqube
$ kustomize build overlays/dev --enable-helm | oc apply -f
```