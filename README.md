# instanciaEc2
# ☁️ Desafio DIO: Gerenciamento de Instâncias EC2 na AWS

## 🧩 Entendendo o Desafio

Este repositório faz parte do **Desafio da DIO (Digital Innovation One)** com foco no **gerenciamento de instâncias EC2 (Elastic Compute Cloud)** na **Amazon Web Services (AWS)**.  
O objetivo é aplicar, na prática, os conhecimentos adquiridos durante as aulas, documentando cada etapa do processo de criação, configuração, monitoramento e segurança de instâncias EC2.

---

## ☁️ O que é o Amazon EC2?

O **Amazon Elastic Compute Cloud (EC2)** é um serviço que oferece **capacidade de computação escalável na nuvem**.  
Ele permite criar e gerenciar **máquinas virtuais** (instâncias) sob demanda, com diferentes configurações de hardware e software.

### 🔹 Principais vantagens:
- Escalabilidade elástica (aumentar ou reduzir recursos conforme a demanda);
- Pagamento sob demanda;
- Integração com diversos serviços da AWS;
- Alta disponibilidade e segurança;
- Suporte a Linux, Windows e outros sistemas.

---

## 🧭 Etapas Realizadas no Laboratório

### 1️⃣ Acesso ao Console AWS
- Login no [AWS Management Console](https://aws.amazon.com/console/);
- Acesso ao serviço **EC2** dentro da seção *Compute*.

### 2️⃣ Criação da Instância
- Clique em **Launch Instance**;
- Escolha de uma **AMI (Amazon Machine Image)** — neste caso, foi usada `Amazon Linux 2`;
- Seleção do **tipo de instância** (`t2.micro` — elegível ao Free Tier);
- Criação de um **par de chaves (.pem)** para acesso SSH;
- Definição de um **Security Group** com regras específicas (porta 22 liberada apenas para IP pessoal);
- Configuração de armazenamento (8 GB SSD);
- Lançamento da instância.

### 3️⃣ Conexão com a Instância
```bash
chmod 400 chave.pem
ssh -i "chave.pem" ec2-user@<IP_PÚBLICO_DA_INSTÂNCIA>
```

-Infelizmente não pude completar essa atividade, por não ter cartão de crédito, nem ter alguem que possa me emprestar.
