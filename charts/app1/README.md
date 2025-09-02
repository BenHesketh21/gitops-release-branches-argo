# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/BenHesketh21/gitops-release-branches-argo
# cd into the cloned directory
git checkout 5c5ed6a570c36609e960af2196e9eb02b6d2c8f7
helm template . --name-template tenant1-app1 --values ./charts/app1/values.yaml --values ./charts/app1/values/test/base.yml --values ./charts/app1/values/test/main/tenant1/version.yml --include-crds
```
