# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/BenHesketh21/gitops-release-branches-argo
# cd into the cloned directory
git checkout d23d06567522a6917c62895a4cb06af54633228e
helm template . --name-template tenant1-app1 --values ./charts/app1/values.yaml --values ./charts/app1/values/test/base.yml --values ./charts/app1/values/test/main/tenant1/version.yml --include-crds
```
