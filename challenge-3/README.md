# Challenge 3 - Terraform

Terraform is a tool for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions.

Terraform is the tool most used for creating infrastructure as Code. this is Infrastructure, described using a high-level configuration syntax. This allows a blueprint of your datacenter to be versioned and treated as you would any other code. Additionally, infrastructure can be shared and re-used.


## Instructions for Jill

Hey Jill,

With our SpaceZ rockets, we should be able to convert the earth back to a green planet in only a few years.
The rockets are ready to launch, but we need to launch the SpaceZ website to track the launch progress.
To do this, you'll have to complete the terraform code.

Important to note is that you only have to change a single file: `appservice.tf`
The corrected file will create a Resource Group, App Service Plan, and the App Service that will host our website.

Now **before you start** open a terminal in vscode (ctrl+shift+\`) and navigate to the folder where you saved the terraform code.
Alternatively, you can also open the folder in your local command prompt / terminal.
When you are in the correct folder (`challenge-3`), run the following command: `az login`

This will open a browser window where you can login to your HTF Azure account.

When you've logged in, come back to the terminal and run the following command: `terraform init`


This will initialize the terraform code. You only have to run this **once**. \
Great, now terraform is ready to go.

After or even before you made some changes in the `appservice.tf` file, you can run the following command to check if the syntax is correct and to see what your code would deploy or alter in the cloud.
- `terraform plan`

If you see any errors, they should guide you in fixing them.

When everything is correct, you can run the following command to apply the changes to the cloud.
- `terraform apply`



After you completed the code successfully, the website will be available on Azure.
Do not forget to fil in your `TeamId` in the appservice.tf file.
Make sure you verify that it works correctly by visiting the website. (check the [Azure portal](https://portal.azure.com) to find its url)


## Prerequisites

1. Install Git: https://git-scm.com/downloads/
2. Install VSCode: https://code.visualstudio.com/
3. Install Azure CLI: https://docs.microsoft.com/en-us/cli/azure/install-azure-cli
4. Install Terraform: https://www.terraform.io/downloads.html
