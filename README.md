# EKS
EKS Install and more 


# INSTALL THE EKS CLIENT TOOLS YOU NEED TO MANAGE EKS CLUSTER 

1. AWSCLI       - 
	curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
	unzip awscliv2.zip
	sudo ./aws/install
	
		Output
		aws --version
	
	
	2. Kubctl                            - Manage EKS 
	curl -o kubectl https://amazon-eks.s3.us-west-2.amazonaws.com/1.18.8/2020-09-18/bin/linux/amd64/kubectl
	chmod +x kubectl 
	sudo cp kubectl /usr/bin/
	
	
																										
	3. IAM Authenticator     - IAM cred to authenticate EKS 
	curl -o aws-iam-authenticator https://amazon-eks.s3.us-west-2.amazonaws.com/1.18.8/2020-09-18/bin/linux/amd64/aws-iam-authenticator
	chmod +x  sudo cp aws-iam-authenticator /usr/bin 
	sudo cp aws-iam-authenticator /usr/bin 
	
	
	4. EKSCTL                          - create cluster EKS up and down 
	curl --silent --location "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp
	cd /tmp
	chmod +x eksctl 
	sudo cp eksctl /usr/bin  
