Terraform Provider
==================

- Website: https://www.terraform.io
- [![Gitter chat](https://badges.gitter.im/hashicorp-terraform/Lobby.png)](https://gitter.im/hashicorp-terraform/Lobby)
- Mailing list: [Google Groups](http://groups.google.com/group/terraform-tool)

<img src="https://cdn.rawgit.com/hashicorp/terraform-website/master/content/source/assets/images/logo-hashicorp.svg" width="600px">

Requirements
------------

-	[Terraform](https://www.terraform.io/downloads.html) 0.12.x
-	[Go](https://developer.fedoraproject.org/tech/languages/go/go-installation.html) 

Building The Provider
---------------------

sudo mkdir $GOPATH
export GOPATH=$GOPATH
go env GOPATH
mkdir -p $GOPATH/src/github.com/terraform-providers
cd terraform-provider-vscale/
go get
go build
mkdir -p ~/.terraform.d/plugins/ 
mv terraform-provider-vscale ~/.terraform.d/plugins/
