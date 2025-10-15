# Projeto Automação com Ansible e Terraform  

Projeto com automação DevOps utilizando boas práticas com **Ansible** e **Terraform** aplicado à **AWS**, desenvolvido durante minha pós-graduação em Multicloud, DevOps e Inteligência Artificial.

---

## Visão Geral  

O projeto está baseado em **aplicação SaaS multi-tenant**, implantada em três estados dos EUA.  
O objetivo foi **automatizar o provisionamento e a configuração completa da infraestrutura** na AWS, utilizando **Terraform** para a criação dos recursos e **Ansible** para a orquestração, configuração e deploy das aplicações em instâncias **EC2**.  

---
## Arquitetura da Solução  

<img width="1098" height="445" alt="image" src="https://github.com/user-attachments/assets/e7a8d9d8-f503-463b-844b-0f9e420413c7" />

O diagrama ilustra o engenheiro DevOps orquestrando a configuração via Ansible e Terraform, o versionamento e a implantação das instâncias EC2 em múltiplos tenants, com backend remoto utilizando **S3** e **DynamoDB** para controle de estado do Terraform.  

---

## ⚙️ Tecnologias Utilizadas  

| Categoria | Ferramenta / Serviço | Função |
|------------|----------------------|--------|
| Automação de Configuração | **Ansible** | Configuração e implantação automatizada das aplicações |
| Infraestrutura como Código | **Terraform** | Provisionamento de EC2, DynamoDB, S3 e IAM Roles |
| Cloud Provider | **AWS (Amazon Web Services)** | Infraestrutura base para execução dos ambientes |
| Armazenamento de Estado | **S3 + DynamoDB** | Backend remoto para controle de estado do Terraform |

---

## Fluxo da Solução  

1. **Terraform** cria automaticamente os recursos AWS (EC2, S3, DynamoDB e IAM Roles).  
2. **Ansible** conecta-se às instâncias EC2 para aplicar as configurações e realizar o deploy da aplicação HumanGov.  
3. Cada “tenant” (estado dos EUA) é provisionado e configurado de forma isolada, garantindo escalabilidade e segurança.  


👨‍💻 Autor
Arlindo Ramos
☁️ Cloud & DevOps Architect | Infraestrutura como Código (IaC) | Automação Cloud
🔗 linkedin.com/in/arlindo-ramos
📧 Contato: arlindoramos.cloud@gmail.com

💬 Automação é o pilar da eficiência em ambientes cloud-native.
