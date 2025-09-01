# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/BenHesketh21/gitops-release-branches-argo
# cd into the cloned directory
git checkout 2ed9f397fd64e91e999501265c50ee2a7f6fa5f8
helm template . --name-template tenant1-app1 --values ./charts/app1/values.yaml --values ./charts/app1/values/test/base.yml --values ./charts/app1/values/test/main/tenant1/version.yml --include-crds
```
