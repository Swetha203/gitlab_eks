# gitlab_eks
These files are related to the Deployment of gitlab docker image in AWS EKS Cluster.
After creating all the files in a directory, to apply the configuration to kubernetes cluster the following commands are used -
 kubectl apply -f .  # This command applies all the file configuration to the kubernetes cluster.
 kubectl apply -f filename   #To apply single file.
 kubectl apply -f file1 -f file2 -f file3   #To apply multiple files at a time.

#To check the created pod status
kubectl get pods -n gitlab #gitlab is the name of namespace that we have created.

#To get the externalIP to access the gitlab on browser
kubectl get svc -n gitlab #gitlab is the name of namespace that we have created. 

