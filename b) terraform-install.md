Terraform Installation
a) Prerequisites

    Install Terraform CLI
    Install AWS CLI
    Install VS Code Editor or any other IDE for writing your code.
    Install HashiCorp Terraform plugin for VS Code - if you are using VS Code.

b) Installation

    You can download the binary for either MACOS or Windows and install on your system

Links:
Download Terraform - choose the appropriate OS:

https://developer.hashicorp.com/terraform/install

Install CLI:

https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html

direct download link for aws-cli:

https://docs.aws.amazon.com/cli/latest/userguide/getting-started-version.html

Microsoft Visual Studio Code Editor:

https://code.visualstudio.com/download

Hashicorp Terraform Plugin for VS Code:

https://marketplace.visualstudio.com/items?itemName=HashiCorp.terraform

AWS CLI Install in macOS:

https://docs.aws.amazon.com/cli/latest/userguide/getting-started-version.html


Install AWS CLI - MAC

    You can alternatively use a package manager = brew for MACOS or Choco for Windows.

   $ brew tap hashicorp/tap
   $ brew install hashicorp/tap/terraform

  or for Windows systems, you can use the command below as an Administrator.
  
  $ choco install terraform -y

You can also follow the procedure below to install terraform on Ubuntu or RHEL
Install Terraform on Ubuntu:

 $sudo apt-get update && sudo apt-get install -y gnupg software-properties-common curl
 $curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -
 $sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
 $sudo apt-get update && sudo apt-get install terraform

Install Terraform on RHEL:

  Install aws cli:

  sudo yum update -y
  
  sudo yum install curl unzip wget -y  
  
  curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
  
  unzip awscliv2.zip
  
  sudo ./aws/install

  Install Terraform:

  a) Download binary

  sudo yum update -y
  
  sudo yum install wget unzip -y
  
  sudo wget https://releases.hashicorp.com/terraform/1.5.5/terraform_1.5.5_linux_amd64.zip
  
  sudo unzip terraform_1.5.5_linux_amd64.zip -d /usr/local/bin
  
  terraform -v

  b) Install from hashicorp repo:

 sudo yum install -y yum-utils
 
 sudo yum-config-manager --add-repo https://rpm.releases.hashicorp.com/RHEL/hashicorp.repo
 
 sudo yum -y install terraform

