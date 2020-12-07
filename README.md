Create a keypair in the desired region of your stack

create 2 elastic ip, one for master and other for node

Run the kube_stack.template file in aws loudformation console

Supply the requested parametes parameters 
KeyPair: keypair name
MasterElasticIP: elastic ip fo master
NodeElasticIP: elastic ip for node
SSHPass: SSH password to login into the VMs, username is exquisapp

Create stack

Check the output to get output parameter such as MasterIP, NodeIP, WorkbenchIP

Login to the master VM with username as "exquisapp" and password supplied at stack creation runtime

run "kubectl get nodes to confirm the the worker node joined to the cluster"



