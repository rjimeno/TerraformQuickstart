# TerraformQuickstart

The content of this repository resulted from following along the A Cloud Guru
training named 'Terraform Quickstart'.

It is useful for reference. Here are some useful commends:

One way to setup the AWS credentials with shell commands like `aws configure
--profile <PROF_NAME>` followed by `export AWS_PROFILE=<PROF_NAME>` where
`<PROF_NAME>` is an arbitrary name of your choice.

After that you may change the current directory to be the location of the
`main.tr` file that uses the modules for the development (`dev`) as follows: `cd
terraform/dev/us-east-1/t2.micro/ec2-deployment/`.

From there you can initialize Terraform, format, validate, and deploy the code
(after carefully reviewing and approving the plan) with the follwing commands:

```
terraform init
terraform fmt
terraform validate
terraform apply
```

Just like the `dev/` directories in the code, you can organize your code for the
test and production environments by copying the `dev/` directories to new
`test/` and `prod/` directories, or by creating them "from scratch".