# Projeto Final Cloud

* código base script terraform: https://learn.hashicorp.com/tutorials/terraform/eks
* código base script ansible: https://medium.com/geekculture/how-to-deploy-the-kubernetes-application-to-aws-eks-using-terraform-and-ansible-7679a3a207a8
* código fonte aplicação: https://fastapi.tiangolo.com/deployment/docker/?h=docker#build-a-docker-image-for-fastapi

Existem dois scripts de implantação (Infraestrutura no padrão Terraform, e Aplicação no padrão Ansible). O script de Terraform irá criar um cluster no serviço AWS EKS configurado com pelo menos 3 instâncias t2.medium. O script Ansible irá efetuar a instalação de uma aplicação Web de uma simples API rodando sob container no cluster EKS criado, rodando em 2 containers/pods, com Autoscaling habilitado e um loadbalancer (ponto de acesso que distribui entre os 2 containers Web). 

O código do script terraform foi baseado no tutorial oferecido pelo próprio terraform e adaptado para os requisitos do projeto.
