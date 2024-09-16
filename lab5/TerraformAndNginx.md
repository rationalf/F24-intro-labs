# Installation

## Version

Terraform v1.9.5
on windows_amd64
+ provider registry.terraform.io/kreuzwerker/docker v3.0.2

## Steps followed to install Terraform

1) Download Chocolaty
2) choco install terraform

## Commands executed to initialize and apply the Terraform configuration

1) mkdir learn-terraform-docker-container
2) cd learn-terraform-docker-container
3) create file main.tf
4) In main.tf:
	terraform {
  required_providers {
    docker = {
      source  = "kreuzwerker/docker"
      version = "~> 3.0.1"
    }
  }
}

provider "docker" {
  host    = "npipe:////.//pipe//docker_engine"
}

resource "docker_image" "nginx" {
  name         = "nginx"
  keep_locally = false
}

resource "docker_container" "nginx" {
  image = docker_image.nginx.image_id
  name  = "tutorial"

  ports {
    internal = 80
    external = 8000
  }
}
5) terraform init
6) terraform apply
7) terraform destroy (when end work)

## Observations or challenges encountered during the installation and deployment process.

1) Need VPN, without him doesn't work anything
2) Install Choco because use windows and exe file don't work

