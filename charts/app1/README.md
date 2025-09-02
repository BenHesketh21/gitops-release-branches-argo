# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/BenHesketh21/gitops-release-branches-argo
# cd into the cloned directory
git checkout dee3fbd958a29d102195f25aa9c7b8151b9aa4bf
helm template . --name-template tenant1-app1 --values ./charts/app1/values.yaml --values ./charts/app1/values/staging/base.yml --include-crds
```
