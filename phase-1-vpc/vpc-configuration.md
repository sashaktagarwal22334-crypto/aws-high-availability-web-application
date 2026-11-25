
# Phase 1: Amazon VPC Configuration

## Objective
Create a custom Virtual Private Cloud (VPC)
to host a highly available AWS web application.

## VPC Details

- VPC Name: Portfolio-VPC
- IPv4 CIDR: 10.0.0.0/16
- Region: Asia Pacific (Mumbai)
- Tenancy: Default

## Subnets

| Subnet | Availability Zone | CIDR |
|---|---|---|
| Public-Subnet-1 | ap-south-1a | 10.0.1.0/24 |
| Public-Subnet-2 | ap-south-1b | 10.0.2.0/24 |

## Internet Gateway

- Name: Portfolio-IGW
- Attached to: Portfolio-VPC

## Route Table

- Name: Portfolio-Public-RT
- Destination: 0.0.0.0/0
- Target: Portfolio-IGW

Both public subnets are associated with
the public route table.

## Outcome

Successfully configured a custom VPC with
two public subnets across separate Availability
Zones and internet routing through an
Internet Gateway.

## AWS Services Used

- Amazon VPC
- Internet Gateway
- Route Tables
- Subnets
