# NextGen AWS Solutions

[![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?logo=amazon-web-services&logoColor=white)](#)

## Projeto

Este repositório apresenta a solução arquitetural para a startup Nova Tech, que visa implementar um e-commerce com foco em **Confiabilidade e Recuperação de Desastres**, seguindo as melhores práticas da AWS. A arquitetura inclui recursos para alta disponibilidade, resiliência e segurança.

---

## Arquitetura Proposta


![Arquitetura](https://github.com/user-attachments/assets/09f995b4-6859-4f69-87f9-6249d2f42838)

### Descrição Geral

A solução utiliza diversos serviços da **AWS** para garantir alta disponibilidade e segurança. O **Route 53 gerencia o DNS**, permitindo balanceamento de carga e failover automático entre regiões. A **Virtual Private Cloud (VPC)** organiza os recursos em subnets públicas e privadas, garantindo controle de tráfego e segurança.

O tráfego é distribuído de forma eficiente pelo **Elastic Load Balancer (ELB)** entre as instâncias do Amazon EC2, que hospedam as aplicações backend. O Amazon RDS, configurado em modo Multi-AZ, oferece alta disponibilidade e replicação de dados. Para backups e arquivos estáticos, o Amazon S3 é usado, garantindo armazenamento escalável e confiável.

Por fim, o controle de acesso é gerenciado pelo **IAM**, com políticas detalhadas que garantem segurança em todos os serviços.

Essa arquitetura segue as melhores práticas da **AWS**, sendo resiliente e preparada para recuperação de desastres.

### Objetivos

- Garantir alta disponibilidade.
- Implementar recuperação de desastres.
- Otimizar custos com um aporte inicial de **US$10.000,00** e gastos recorrentes de até **US$500,00/mês**.

### Principais Componentes

#### Subnets
- **Subnets Públicas**: Serviços com acesso à internet (ELB, NAT Gateway).
- **Subnets Privadas**: Recursos internos como bancos de dados (Amazon RDS).

#### Balanceamento de Carga
- O ELB distribui o tráfego entre as instâncias EC2 em diferentes zonas de disponibilidade, garantindo escalabilidade automática.

#### Recuperação de Desastres
- **Replicção Multi-Região** 🌍: O banco de dados RDS é replicado para uma região secundária para mitigar falhas.

---




## Tecnologias Utilizadas

- [Amazon Route 53](https://aws.amazon.com/route53/)
- [Amazon EC2](https://aws.amazon.com/ec2/) 
- [Amazon RDS](https://aws.amazon.com/rds/) 
- [Amazon S3](https://aws.amazon.com/s3/)
- [Elastic Load Balancer](https://aws.amazon.com/elasticloadbalancing/)
- [IAM](https://aws.amazon.com/iam/) 

---

## Equipe

- [DenianRamos](https://github.com/DenianRamos)
- [Breno-ds-263](https://github.com/Breno-ds-263)
- [RebecaOuriques](https://github.com/RebecaOuriques)
- **Lucas Oliveira**
- **Pamela Carvalho**


---

## Referências

- [Calculadora AWS](https://calculator.aws/#/estimate?id=05ac4890200f41f7a6aeaba7d2e3041346abdb14)

