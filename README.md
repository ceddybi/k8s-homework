## Workflow
- First set up the cluster with terraform like below
- Update CI configuration with k8 cluster information
  
## Deployment mechanism
A push to `master` branch should start a github action, that builds the docker images, pushes it to ECR, after it updates the deployment in k8s with the new docker image.


To run this example you need to execute:

```bash
$ cd terraform
$ terraform init
$ terraform plan
$ terraform apply
```