# Basic provisioning of EKS with Terraform

You can provision a basic EKS cluster with Terraform with the following commands. Just copy this folder locally & execute below commands

```bash
terraform init
terraform plan
terraform apply
```

It might take a while for the cluster to be creates (up to 15-20 minutes).

As soon as cluster is ready, you should run the following command to configure your kubectl
`      aws eks --region $(terraform output -raw region) update-kubeconfig  --name $(terraform output    -raw cluster_name)
`
