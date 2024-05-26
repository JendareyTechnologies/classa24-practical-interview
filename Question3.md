===================================================================
# Question3

-We will be using killercoda free servers for today's practical session:

-Go to the below webpage and sign on with your Github account.   

https://killercoda.com/

===================================================================

# Time 15: mins 

-Set your time by google searching the below:

-google timer 15 minutes countdown


# Note: Copy and Paste the answers to the group chat

-Look for and click on kubernetes and select Playground - Play with kubernetes

-or 

-use the below URL:

https://killercoda.com/kubernetes/scenario/playground

# Perform the below task

# Question 1:
How many nodes are in the cluster?

# Question 2:
What is the node or nodes OS-IMAGE?

# Question 3:
What is the CONTAINER_RUNTIME installed on the cluster?

# Question 4:
What is the Container Network Interface (CNI) installed on the cluster?

# Question 5:
How many depolyment are in the kube-system - namespace? 

# Question 6:
How many sevices are currently running in the whole cluster and what are these services called? 

----

-Hint:

-kubectl get nodes -o wide

-kubectl get all -A


============================================================

# Question 2:

-Using the below kubernetes documentation link

https://kubernetes.io/docs/concepts/workloads/controllers/deployment/

- Deploy ten replicas of a webpage called: - "nginx-deployment" using an image called: nginx:1.14.2


-Hint:

-vim

-kubectl apply -f nginx-web.yaml

-kubectl get deployment
  
-kubectl get all

============================================================
