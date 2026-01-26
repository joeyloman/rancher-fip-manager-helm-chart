# rancher-fip-manager Helm Chart

## Prerequisites

- Helm 3.x

## Adding the Chart

```SH
helm repo add rancher-fip-manager https://joeyloman.github.io/rancher-fip-manager-helm-chart
helm repo update
```

## Installing the Charts

### rancher-fip-manager applications

Note: install this in the Rancher Local cluster.

```SH
helm install rancher-fip-manager rancher-fip-manager/rancher-fip-manager -n rancher-fip-manager --create-namespace
```

### rancher-fip-lb-controller

Note: install this in the downstream clusters.

```SH
helm install rancher-fip-lb-controller rancher-fip-manager/rancher-fip-lb-controller -n rancher-fip-manager --create-namespace
```

# License

Copyright (c) 2026 Joey Loman <joey@binbash.org>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

[http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
