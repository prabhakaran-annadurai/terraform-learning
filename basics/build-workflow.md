## Basic Build workflow

**Azure environment**

step1 - Set Environment variables for login:

- Depending on the target cloud environment
- For Azure following are required,
  ARM_CLIENT_ID, ARM_CLIENT_SECRET, ARM_SUBSCRIPTION_ID, ARM_TENANT_ID


step2 - terraform init
- downloads required providers
- connects to backend (default is local)

step3 - terraform fmt
- formats all files in the directory

step4 - terraform validate
- only to validate the syntax
- not for validating variables and their values

step5 - terraform apply
- calls "terraform plan" first
- lists details on what's going to be applied
- prompts a confirmation before applying the changes

step6 - terraform state list
- provides list of resources managed in the given workspace
- can view a particular resource by "terraform state show *resource_name*"

Screenshots:


![](../screenshots/screenshot-1.png)
<br><br>
![](../screenshots/screenshot-2.png)