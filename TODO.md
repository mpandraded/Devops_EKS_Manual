# VPC
- VPC
- Subnet Publica
- Subnet Privada
  - Precisa se conectar à internet, sem estar disponivel para internet. (NAT)
- IG
- NAT
- SG
- Route Table

# Host do Cassandra *
- 3 hosts
- Instala cassandra
- Já temos o arquivo de configuracao padrao.
- Subnet Privada
- Type:
  - C5.large
  - 100gb storage
  - TODO: avaliar montar EFS

# EFS *
- File system disponível para toda VPC

# MySQL (RDS) *
- Disponível para toda VPC

# EKS *
- Policies
  - EBS
  - EFS
  - cert-manager
  - external-dns
  - awsLoadBalancerController
  - autoScaler
  - imageBuilder
- Plugins
  - ebs-csi driver
  - efs-csi driver
  - ingress nginx
  - external-dns
  - cert-manager
  - cluster-issuer (letsencrypt)

[*] Applications
- API
- Developer Portal

### Prefered Region
eu-west-1 (Ireland)