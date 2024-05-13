# fluxcd-demo

flux bootstrap git \
  --url=ssh://git@github.com/teochenglim/fluxcd-demo \
  --branch=main \
  --private-key-file="~/.ssh/id_rsa" \
  --path=clusters/local-cluster


mkdir -p fluxcd-demo/clusters/my-cluster/{flux-system,namespaces,workloads,services,configmaps,secrets,other-resources}
