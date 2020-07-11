# Learning Terraform

Creating some terraform samples as tutorials for myself.


## Basics of running terraform

- You initalise terraform

```bash
terraform init
```

- You run a terraform validate

```bash
terraform validate
```

- You run a terraform plan

```bash
terraform plan
```

- You run a terraform apply

```bash
terraform apply
```

- You run a terraform destroy

```bash
terraform destroy
```

Additional terraform commands

```bash
terraform import azure_resource_group rg_function_name
```

## Listing Azure VM Images

Run the following command:

```powershell
az vm image list-skus  --publisher MicrosoftWindowsServer --location southeastasia --offer windowsserver
```

You should get something similar to :

```bash
Location       Name
-------------  ----------------------------------------------
southeastasia  2008-R2-SP1
southeastasia  2008-R2-SP1-smalldisk
southeastasia  2008-R2-SP1-zhcn
southeastasia  2012-Datacenter
southeastasia  2012-Datacenter-smalldisk
southeastasia  2012-Datacenter-zhcn
southeastasia  2012-R2-Datacenter
southeastasia  2012-R2-Datacenter-smalldisk
southeastasia  2012-R2-Datacenter-zhcn
southeastasia  2016-Datacenter
southeastasia  2016-Datacenter-Server-Core
southeastasia  2016-Datacenter-Server-Core-smalldisk
southeastasia  2016-Datacenter-smalldisk
southeastasia  2016-Datacenter-with-Containers
southeastasia  2016-Datacenter-with-RDSH
southeastasia  2016-Datacenter-zhcn
southeastasia  2019-Datacenter
southeastasia  2019-Datacenter-Core
southeastasia  2019-Datacenter-Core-smalldisk
southeastasia  2019-Datacenter-Core-with-Containers
southeastasia  2019-Datacenter-Core-with-Containers-smalldisk
southeastasia  2019-Datacenter-smalldisk
southeastasia  2019-Datacenter-with-Containers
southeastasia  2019-Datacenter-with-Containers-smalldisk
southeastasia  2019-Datacenter-zhcn
southeastasia  Datacenter-Core-1803-with-Containers-smalldisk
southeastasia  Datacenter-Core-1809-with-Containers-smalldisk
southeastasia  Datacenter-Core-1903-with-Containers-smalldisk
```

## User names and passwords

Run the following command to get the usernames and passwords for my virtual machine:

```bash
./passwords.sh
```

You should see output similar to:

```bash
Username is: myuser
Password is: mypassword
```

az vm show -d -g resourceGroupName -n vmName --query publicIps -o tsv

printenv TF_VAR_vm_admin_username
printenv TF_VAR_vm_admin_password
