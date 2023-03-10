# AWS-Terraform-VPN-transit-gateway
This GitHub repository contains a Terraform script that sets up a Transit Gateway (TGW) on AWS. A TGW enables communication between multiple VPCs and on-premises networks using a VPN (Virtual Private Network) connection. The script can be used to automate the creation and configuration of the TGW and the necessary components such as VPN connections, customer gateways, and routing. The script also creates VPN attachments for each of the VPCs which need to be connected to the Transit Gateway.

Read more about this particural VPN setup - URL to be advertised


# File structure
- ec2.tf : Creates EC2 instance (just for testing).
- outputs.tf : This file contains the outputs that are returned after the Terraform script is run - Peer IP addresses for two VPN connections and EC2 instance private IP.
- provider.tf : This file containts root module of the script which is provider configurations
- transit.tf : Creates the TGW and the necessary components such as VPN connections, customer gateways, and routing. The script also creates VPN attachments for each of the VPCs which need to be connected to the Transit Gateway.
- vars.tf : This file contains the values for the variables that are used in the script - VPN parameteres, VPC settings etc.
- vpc.tf : Creates VPC.
- vpn.tf : Creates two VPN connections.
- README.md : This file contains the documentation for the repository.
