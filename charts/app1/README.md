# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/BenHesketh21/gitops-release-branches-argo
# cd into the cloned directory
git checkout 02310bcf1f945d61dc2b133874bef507bdc111d6
helm template . --name-template tenant1-app1 --values ./charts/app1/values.yaml --values ./charts/app1/values/test/base.yml --values ./charts/app1/values/test/main/tenant1/version.yml --include-crds
```
