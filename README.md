# Simple Kubernetes deployment generation using Jsonnet

## Local Dependencies to run example
* [Jsonnet](https://jsonnet.org/)
* [Jsonnet Bundler](https://github.com/jsonnet-bundler/jsonnet-bundler)
* [yq](https://mikefarah.gitbook.io/yq/)

## Example
```bash
cd examples/spring-boot
jb install
jsonnet -J vendor k8s-manifest.jsonnet | yq r --prettyPrint -
```
