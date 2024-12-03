```
helm repo add metallb https://metallb.github.io/metallb
helm install metallb metallb/metallb

k apply -f ip-address-pool.yaml -f l2-advertisement.yaml
```

Provides a pool of IP addresses and advertises them to L2 network for ingress controller to pick up.
