# cka-prep-by-hari
This is the repo for prep and clearing CKA exam easily.

**Installation steps:**

To start with CKA preparation as it is a lab exam, we would need to have the cluster setup and an easy way to do it is using Kind.

Below are the steps to be followed for creating the cluster using Kind.

1) We need to have **go** and **docker/podman** installed as a pre-requisite for the same.
2) Using go we can install kind and then using kind we can install the cluster as shown below.
   1) Install **go** using the installation steps mentioned on their website: https://go.dev/doc/install
   2) Install <a href="https://www.docker.com/">Docker </a> or <a href="https://podman.io">Podman </a> as this is also a required step before installing Kind. 
   3) Install **Kind** using the steps based on your OS as shown on this website: https://phoenixnap.com/kb/kubernetes-kind
3) To check if the installation was successful by running the below commands
   1) go version should give some similar output based on the version installed.
      Execute the below command in Terminal.

      **go version**
      <img width="489" alt="image" src="https://github.com/harikishan468/cka-prep-by-hari/assets/18546196/27140578-37ce-4dc4-ae42-431b8e904f40">
   3) Kind version should give output based on the version installed.
      Execute the below command in Terminal.

      **kind version**
      <img width="489" alt="image" src="https://github.com/harikishan468/cka-prep-by-hari/assets/18546196/59b7cf74-84c5-4796-834a-9c4a71ed5dac">
   4) To check if Docker is installed properly or not, check using the below command.
      **docker version**
      <img width="556" alt="image" src="https://github.com/harikishan468/cka-prep-by-hari/assets/18546196/e637e3d5-c6cc-4a05-911b-ecfdef8a2cfb">
4) Once the above step is successful, then create a cluster using the below command.
      **kind create cluster**
      <img width="945" alt="image" src="https://github.com/harikishan468/cka-prep-by-hari/assets/18546196/f0fcc074-5a2f-4b3b-add3-de3681a47e47">
5) Use the below command to get the cluster info.
     **kubectl cluster-info --context kind-kind**
     **Kubernetes control plane is running at https://127.0.0.1:<PORTNO>
     CoreDNS is running at https://127.0.0.1:<PORTNO>/api/v1/namespaces/kube-system/services/kube-dns:dns/proxy
     To further debug and diagnose cluster problems, use 'kubectl cluster-info dump'.**




