# Namespace

- Provides a mechanism to group resources within  cluster
- There are 4 initial namespaces:
  - `default`: Default namespace for resources
    - `kube-system`: Contains system services and components
    - `kube-public`: Read-only namespace for public resources
    - `kube-node-lease`: Manages node lease objects

**NOTE:** By default, namespaces DO NOT act as a network/security boundary.

## Creating a Namespace

```yaml
apiVersion: v1
kind: Namespace
metadata:
    name: my-namespace
```
