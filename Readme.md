Learning kubernetes for Container orchstration on local machine and on cloud platforms


#Set Up K8s Cluster on local machine.
1. Download Docker from the official website and install. https://www.docker.com/products/docker-desktop/
   i. Start the docker and confirm its up and running without issues(**Engine Running**).
   ii. Create docker hub account(if ypu don't have one) https://hub.docker.com/signup
2. Download Minikube and kubectl binaries, add them to the path on enviromental Variables(for windows)
   i. for minikube https://minikube.sigs.k8s.io/docs/start/
   ii. for kubectl https://kubernetes.io/docs/tasks/tools/install-kubectl-windows/(other OS https://kubernetes.io/docs/tasks/tools/)
- Confirm that all is working with minkikube version and kubectl version
3. Create a single node cluster to get the understanding of K8s and deploy a spring application.
 Open the terminal(powershell,Bash,cmd etc...)
 Run
 - **minikube start**(or Minikube start --driver=docker)
  To confirm the cluster is up, Run minikube status(It should show running.)
 - **kubectl get nodes** (minikube   Ready    control-plane,master   1min   v1.23.3)
 Open the dashboard on browser
 - **minikube dashboard --url**
 (You will be required to install the dashboard plane on the cluster. 
 kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.7.0/aio/deploy/recommended.yaml)
 
Congratulations👏👏👏!!! you've just created A Kuberneetes Cluster and ready to deploy containerized applications of any language.
