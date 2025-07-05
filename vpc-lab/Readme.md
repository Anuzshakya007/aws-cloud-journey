# AWS Custom VPC Project

This project demonstrates how I built a custom VPC from scratch using the AWS Console, including public and private subnets, route tables, and an EC2 instance in a public subnet.

## VPC Structure

- VPC CIDR: 10.0.0.0/16
- Public Subnet: 10.0.1.0/24
- Private Subnet: 10.0.2.0/24
- Internet Gateway: attached to public subnet
- Route Table: custom table with 0.0.0.0/0 via IGW

## VPC CIDR Plan

| Resource         | Name               | CIDR Block       | AZ                 | Notes                         |
|------------------|--------------------|------------------|--------------------|-------------------------------|
| VPC              | my-vpc-01		| 10.0.0.0/16      | N/A                | Root VPC block                |
| Public Subnet    | public-subnet-01   | 10.0.1.0/24      | us-east-1a		| Public access, IGW attached   |
| Private Subnet   | private-subnet-01  | 10.0.2.0/24      | us-east-1a   	| For internal workloads        |
| Internet Gateway | internet-gateway-01| —                | —                  | Enables outbound internet     |
| Route Table      | public-route-table | —                | —                  | Public subnet routing via IGW |

## Tools Used
- AWS VPC, Subnet, IGW, Route Table
- Amazon EC2
- Security Groups

## Learnings
- How AWS networking is structured
- The difference between public and private networks
- Basics of route tables and gateways

