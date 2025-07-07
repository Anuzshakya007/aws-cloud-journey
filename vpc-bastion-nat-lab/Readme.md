# 🔐 AWS Bastion Host + NAT Gateway + Private Subnet Lab

## ✅ Objective

- Securely SSH into a private EC2 instance using a Bastion Host
- Enable outbound internet access for private instances using a NAT Gateway
- Practice IAM-free VPC architecture

## 🧱 Architecture

| Component        | Value	                      |
|==================|==================================|
| VPC CIDR         | 10.0.0.0/16              	      |
| Public Subnet    | 10.0.1.0/24              	      |
| Private Subnet   | 10.0.2.0/24              	      |
| Bastion Host     | EC2 in public subnet     	      |
| Private EC2      | EC2 in private subnet    	      |
| NAT Gateway      | Public subnet with EIP   	      |
| Route Table      | Private subnet routed via NAT GW |

📌 *All security groups scoped to least privilege.*

## 🔐 What I Learned

- How to isolate EC2s in private subnets
- How Bastion Hosts act as secure jump points
- How NAT Gateways enable internet access without public IPs
- How to route traffic securely across AWS VPC layers

## 🧪 Validated

- SSH from laptop → Bastion Host → Private EC2
- `apt update` and `ping google.com` from private EC2

