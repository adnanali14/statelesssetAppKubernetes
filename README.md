# statelesssetAppKubernetes
Deploy a Stateless Application in a Kubernetes Cluster
Kubernetes Cluster

Kubernetes is a popular orchestration tool for managing containerized applications. Kubernetes is production-ready and used by enterprises around the world. With Kubernetes, you can automatically deploy, scale, rollout updates, rollback, and recover container applications.
Upon completion 

Set up a Kubernetes master node
Set up a Kubernetes worker node
Deploy a stateless application in a Kubernetes cluster
Create a Kubernetes service to allow access to the application from outside the cluster
Effectively manage Kubernetes clusters from the command-line
In the first  Step, wil configured a Red Hat Enterprise Linux server as a Kubernetes control plane node and then will used the yum package manager to install all of the dependencies and modified the configuration files to suit the needs of this proj Also verified the API server was up and running and added a node resource to the cluster.
Kubernetes worker nodes, or simply nodes, provide the runtime environment for Kubernetes. Nodes maintain running pods in the Kubernetes cluster. Kubernetes clusters can have one node to thousands of nodes. Each node is configured with several components:

kubelet: Primary agent of the node.  Responsible for watching pods assigned to it, running the pod's containers, reporting pod status, etc.
kube-proxy: Enables the Kubernetes service abstraction by maintaining network rules and connection forwarding
Docker: Runs containers
This will use Docker for running containers, although Kubernetes supports other container technologies. The control plane node in a Kubernetes cluster can also perform worker node tasks and therefore worker node components are also installed on control plane nodes. 

With a Kubernetes cluster up and running, you can deploy an application in the cluster. we will use a Docker image of a game for the application. The application runs in a client web browser and doesn't store any state across sessions. 
 
