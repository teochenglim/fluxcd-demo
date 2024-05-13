# fluxcd-demo


```shell
brew install fluxcd/tap/flux
flux check --pre
flux install

flux bootstrap git \
  --url=ssh://git@github.com/teochenglim/fluxcd-demo \
  --branch=main \
  --private-key-file="~/.ssh/id_rsa" \
  --path=clusters/local-cluster


mkdir -p fluxcd-demo/clusters/my-cluster/{flux-system,namespaces,workloads,services,configmaps,secrets,other-resources}

```