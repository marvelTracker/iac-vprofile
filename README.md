# Terraform code

## Maintain vpc & eks with terraform for vprofile project

## Tools required

Terraform version 1.6.3

### Steps

- terraform init
- terraform fmt -check
- terraform validate
- terraform plan -out planfile
- terraform apply -auto-approve -input=false -parallelism=1 planfile

####

#####

####

Clean Up resources
`/iac-vprofile/terraform> kubectl delete -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/cloud/deploy.yaml`

`/iac-vprofile/terraform> terraform init -backend-config="bucket=vprofileactionsXX"`

`/iac-vprofile/terraform> terraform destroy`
