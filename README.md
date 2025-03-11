Terraform Provisioners

Provisioners can be used to model specific actions on the local machine or on a remote machine in order to prepare servers or other infrastructure objects for service.

To this point the EC2 web server we have created is useless. We created a server without any running code with no useful services are running on it.

We will utilize Terraform provisoners to deploy a webapp onto the instance we've created. 
In order run these steps Terraform needs a connection block along with our generated SSH key from the previous labs in order to authenticate into our instance. 
Terraform can utilize both the local-exec provisioner to run commands on our local workstation, 
and the remote-exec provisoner to install security updates along with our web application.

1: Upload your SSH keypair to AWS and associate to your instance.
2: Create a Security Group that allows SSH to your instance.
3: Create a connection block using your SSH keypair.
4: Use the local-exec provisioner to change permissions on your local SSH Key
5: Create a remote-exec provisioner block to pull down and install web application.
6: Apply your configuration and watch for the remote connection.
7: Pull up the web application and ssh into the web server (optional)
