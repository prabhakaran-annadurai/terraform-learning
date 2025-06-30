## Basic change workflow

### 1. Adding a new resource

- step1 : Adding config code in main.tf file
- step2 : run "terraform apply"

Eg. I created a new vnet in an existing resource group 


![](../screenshots/screenshot-3.png)


### 2. Changing an existing resource


Terraform compares existing state with new changes proposed before applying

Eg. added a tag to an existing resource group


![](../screenshots/screenshot-4.png)

### 3. Review updated state

- terraform state list -> gives list of all resources managed in this workspace

- terraform show -> shows all properties tracked for a particular resource group


![](../screenshots/screenshot-5.png)