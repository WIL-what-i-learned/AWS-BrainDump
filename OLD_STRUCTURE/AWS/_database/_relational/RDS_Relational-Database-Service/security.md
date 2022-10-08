# RDS - SECURITY

- Layers
    - Network Isolation
    - IAM for access control
    - encryption at rest
    - SSL for database connectivity

## Network Isolation

> Virtual Private Cloud (VPC)

- Private Subnet: make it security from public routes on the internet
- Security Group: database instance firewall protection so you can securely control network configuration
- Public Accessibility: turn off public accessibility to restrict access outside the VPC
- ClassicLink: use network with non-VPC resources
- DirectConnect: replicate with on premise database
- VPC Peering: share between VPCs
- Security Group

## Access Control

> IAM

## Encryption at Rest

> 

- no performance impact
- all connected DBs & backups are encrypted
- access to keys is logges
- can rotate keys but you cant unencrypt once you encrypt
- Two Tier Encryption: master keys created by you each instance with its own data key 

## SSL Connectivity

- nobody can intercept
- enforce SSL via Parameter Groups
