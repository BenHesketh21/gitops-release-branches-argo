# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/BenHesketh21/gitops-release-branches-argo
# cd into the cloned directory
git checkout 1fa1951f167fc51506cc67146ca757b6414b81d9
helm template . --name-template tenant1-app2 --values ./charts/app2/values.yaml --values ./charts/app2/values/test/base.yml --values ./charts/app2/values/test/main/tenant1/version.yml --include-crds
```
