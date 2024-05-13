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


mkdir -p clusters/local-cluster/{flux-system,namespaces,local,other-cluster}
mkdir -p clusters/local-cluster/local/{workloads,services,configmaps,secrets,other-resources}

```