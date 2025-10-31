# 🚀 Desafio de Projeto DIO: Infraestrutura como Código com AWS CloudFormation

Olá! Este repositório é o entregável do desafio de projeto da **Digital Innovation One (DIO)** focado na implementação e documentação de uma infraestrutura automatizada usando **AWS CloudFormation**.

Aqui demonstro os conceitos aprendidos e minha experiência prática com a automação de recursos na AWS.

---

## 🎯 **Objetivos de Aprendizagem e Implementação**

O objetivo principal deste laboratório foi aplicar a filosofia **Infrastructure as Code (IaC)**, utilizando a ferramenta nativa da Amazon Web Services.

### 💡 **Conceitos Abordados:**

* **Infraestrutura como Código (IaC):** Entendimento de como gerenciar e provisionar recursos de infraestrutura por meio de arquivos de configuração.
* **AWS CloudFormation:** Utilização de templates em YAML (ou JSON) para descrever e provisionar recursos AWS de forma declarativa.
* **Gestão de Stacks:** Criação, atualização e exclusão de conjuntos de recursos (Stacks) de maneira organizada e repetível.
* **Organização e Documentação:** Utilização do Git e GitHub para versionamento e documentação técnica.

### ⚙️ **Recursos AWS Provisionados:**

**Nesta implementação, o CloudFormation foi responsável por provisionar a seguinte arquitetura:**

* *\[**SEU RECURSO PRINCIPAL** - Ex: Uma Virtual Private Cloud (VPC) personalizada.]*
* *\[**SEU RECURSO SECUNDÁRIO** - Ex: Um Subnet público.]*
* *\[**SEU RECURSO TERCIÁRIO** - Ex: Um Security Group que permite acesso SSH (Porta 22) e HTTP (Porta 80).] *
* *\[**SEU RECURSO QUATERNÁRIO** - Opcional, Ex: Uma instância EC2 t2.micro rodando Amazon Linux.]*

---

## 📂 **Estrutura do Repositório**

Este repositório está organizado para facilitar a visualização do código e da documentação:

* **`README.md`:** O arquivo que você está lendo, contendo todos os insights, a descrição do processo e os aprendizados.
* **`/templates/`:** Pasta contendo o template YAML/JSON do CloudFormation utilizado.
    * `cloudformation-template.yaml` *(ou `.json`):* O código fonte da minha infraestrutura.
* **`/images/`:** Pasta com capturas de tela dos recursos provisionados na AWS.

---

## 💻 **O Template do CloudFormation**

O coração deste projeto é o arquivo de template, onde toda a infraestrutura é declarada.

### **Insights sobre a Construção do Template:**

* Utilizei a linguagem **YAML** por sua maior legibilidade.
* A seção **`Resources`** é a parte crucial, onde cada recurso AWS é mapeado.
* Usei **`Parameters`** para tornar o template mais flexível (ex: para definir o tipo de instância ou o bloco CIDR da VPC).
* Usei **`Outputs`** para retornar informações importantes após a criação da Stack (ex: o ID da VPC criada ou o DNS Público da EC2).
