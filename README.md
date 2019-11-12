# cloud-developer
Project 3 Udacity Cloud Developer

To Deploy:
- Go to the courses-03/exercises/udacity-c3-deployment folder
- Follow instructions in the README to setup dependencies
- From the .aws folder:
    - terraform init
    - terraform plan
    - terraform apply
- This creates your kubernetes cluster, to configure it go up one directory and enter the following: `kubeone install config.yaml --tfjson aws/`
- To run the containers:
    - Replace the default variables in your aws-secret.yaml and env-secret.yaml files with your own secrets. 
    - Configure env-configmap to point to your own containers
- Run `kubectl apply -f .` to run all services 
