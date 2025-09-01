# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/BenHesketh21/gitops-release-branches-argo
# cd into the cloned directory
git checkout 04c6e2e539c08c6b686dd5c5928345bd14d179de
helm template . --name-template tenant1-app1 --values ./charts/app1/values.yaml --values ./charts/app1/values/staging/base.yml --include-crds
```
