# Pod

- The "smallest deployable unit"
- Represents a set of running containers on your cluster
- Can contain one or more containers.
- All containers in a pod share:
  - Network (IP address and port space)
  - Storage (volumes)
  - Specification for how to run the containers
- Pods are ephemeral and disposable
  - If a pod dies, it won't be resurrected
    - New pods are created to replace them
- Pods are usually managed by higher-level controllers like Deployments, StatefulSets, or Daemon.
- Within a pod, you can have the following types of containers:
  - **Application containers**: The main containers that run your application.
    - **Init containers**: Special containers that run before the application containers start. They can perform setup tasks like initializing databases or waiting for services to be available.
    - **Sidecar containers**: Containers that run alongside the main application containers to provide additional functionality, such as logging, monitoring, or proxying.

## Pods configuration

- Listening ports
- Health probes
- Resource limits and requests
- Volumes mount
- Environment variables
- Security context
- Image pull secrete
- DNS Policies
- Node selector
- Affinity and anti-affinity rules
- Tolerations
- Restart policy
- Service account
- Labels and annotations
