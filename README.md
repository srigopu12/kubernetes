KUBERNETES--
     Kubernetes, often abbreviated as K8s, is an open-source container orchestration platform designed to automate the deployment, scaling, and management of containerized applications. Originally developed by Google and later donated to the Cloud Native Computing Foundation (CNCF), Kubernetes has become the de facto standard for managing containerized workloads in production environments.

The architecture of Kubernetes is designed to provide a scalable, resilient, and extensible platform for container orchestration. It consists of several components that work together to manage containerized workloads efficiently. Here's an overview of the Kubernetes architecture:

Master Node:

 1.API Server: The central management component that exposes the Kubernetes API, which serves as the primary interface for users, administrators, and controllers to interact with the cluster.
 2.Scheduler: Responsible for scheduling Pods onto available worker nodes based on resource requirements, affinity/anti-affinity rules, and other constraints.
Controller Manager: A collection of controllers that regulate the state of the cluster, ensuring that the desired state matches the actual state. Controllers include the Node Controller, Replication Controller, Endpoint Controller, and Service Account and Token Controller.
 3.etcd: A distributed key-value store that stores the cluster's configuration data, state, and metadata. etcd provides a consistent and highly available data store, serving as the single source of truth for the cluster.
Worker Nodes (Minions):

   1.Kubelet: An agent that runs on each node and is responsible for maintaining the state of the node, communicating with the API server, and managing Pods and containers on the node.
   2.Container Runtime: The software responsible for running containers. Kubernetes supports various container runtimes, including Docker, containerd, and CRI-O.
   3.Kube-proxy: Maintains network rules on nodes, enabling communication between Pods and external clients. Kube-proxy implements services, load balancing, and network policy enforcement.
