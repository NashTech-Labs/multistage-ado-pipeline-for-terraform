# multistage-ado-pipeline-for-terraform
This techub contains the multi-stage azure devops pipeline for terraform (having stages for terraform init, terraform fmt, terraform vaildate, terraform  plan, terraform apply and terraform destroy)

## Steps for execution:

- clone repo
- go to azure devops
- go to the project where to create the pipeline
- go to library and create a variable group 'tf-variables' with following key-value pairs:
  - client_id: value for the client id of the service principal (azure)
  - client_secret: value for the client secret of the service principal (azure)
  - tenant_id: value for the tenant id of the service principal (azure)
- go to pipeline import existing yaml of the pipeline