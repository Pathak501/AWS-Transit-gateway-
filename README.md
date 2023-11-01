# AWS-Transit-gateway- 
##What is a Transit gateway?
The AWS Transit Gateway helps you connect multiple VPCs and on-premises networks through a central hub. It simplifies your network with VPCs and on-premises connections and solves the problem of complex peering relationships.
With VPC peering using the Transit gateway, your data is always encrypted and no longer uses the public internet for communication.

##Benefits of using Transit gateway:

Easy to connect
Full control
Greater security
Multicast feature

##Reasons to use Transit gateway over VPC peering:
VPC peering does not support transitive peering, meaning you can only peer two VPC at a time.
To peer your VPC with an on-premise network, you can not use VPC peering. Transit gateway supports connecting on-premise networks.
Transit gateway limits:
Per transit gateway, you can have 20 transit gateway route tables.
Per transit gateway, you can have 10000 routes.
Per transit gateway, there can be 50 transit gateway attachments.
Per VPC, you can have 5 unique transit gateways.

## Pre-requisite for this lab
you must have AWS Account
Basic knowladge of EC2, VPC and Networking concept.

## Task You have to done
sign in AWS account than First of all you have to create first VPC with VPC and more option (just becouse it is easy if u want to go with old option u can..,)
AfterCreate a Public subnet in First VPC
Create and attach an Internet Gateway
Create a Public Route Table and associate it with the subnet
Add public Route in the Route table
Launch an EC2 instance in public subnet
Create a Second VPC
Create a Private subnet in Second VPC
Launch an EC2 instance in Second VPC
Create a Transit gateway
Create two Transit gateway attachment for the VPCs created
Add the routes in the First VPC’s route table
Add the routes in the Second VPC’s route table
Test the connectivity between two VPCs
