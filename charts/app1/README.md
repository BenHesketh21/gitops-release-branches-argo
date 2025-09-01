# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/BenHesketh21/gitops-release-branches-argo
# cd into the cloned directory
git checkout e5cd38af7f0af75c9ede0085ea6af9b8620d7aab
helm template . --name-template tenant1-app1 --values ./charts/app1/values.yaml --values ./charts/app1/values/test/base.yml --values ./charts/app1/values/test/main/tenant1/version.yml --include-crds
```
