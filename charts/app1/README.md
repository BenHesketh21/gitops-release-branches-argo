# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/BenHesketh21/gitops-release-branches-argo
# cd into the cloned directory
git checkout fe72bab1807c0455bf3492c9f68408963f8b86d5
helm template . --name-template tenant1-app1 --values ./charts/app1/values.yaml --values ./charts/app1/values/staging/base.yml --include-crds
```
