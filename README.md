# Kustomization

## RUN
```
kustomize create --resources hello/overlay/staging
kustomize build . > s-deploy.yaml
kubectl apply -f s-deploy.yaml
```

```
kustomize create --resources hello/overlay/production
kustomize build . > p-deploy.yaml
kubectl apply -f p-deploy.yaml
```

## References
* https://kubernetes.io/docs/tasks/manage-kubernetes-objects/kustomization/
