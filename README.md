# Configuração de Instância Gerenciada do Azure SQL

Este guia descreve os passos necessários para configurar uma instância gerenciada do banco de dados Azure SQL utilizando o Portal do Azure.

## Requisitos

Antes de iniciar, certifique-se de que você tem:

- Uma conta ativa no [Portal do Azure](https://portal.azure.com)
- Permissões suficientes para criar recursos (como administrador ou colaborador)
- Um grupo de recursos (ou permissão para criar um)

## Passos para criar a instância gerenciada

### 1. Acessar o Portal do Azure

1. Acesse o [Portal do Azure](https://portal.azure.com)
2. No menu de navegação à esquerda, selecione **"Criar um recurso"**

### 2. Iniciar a criação da instância

1. Pesquise por **Instância Gerenciada do Azure SQL**
2. Clique em **"Instância Gerenciada do Azure SQL"** e depois em **"Criar"**

### 3. Preencher informações básicas

Na guia **Básico**, forneça as seguintes informações:

- **Assinatura**: selecione a sua assinatura do Azure
- **Grupo de Recursos**: selecione um existente ou crie um novo
- **Nome da Instância**: escolha um nome exclusivo para a instância
- **Região**: escolha a região onde a instância será implantada
- **Camada de preço**: escolha entre General Purpose ou Business Critical
- **Contagem de vCores**: defina conforme necessidade
- **Tamanho de armazenamento**: defina em GB
- **Autenticação do administrador**: configure o login e senha do administrador SQL

### 4. Configurações de rede

- Escolha uma **rede virtual** existente ou crie uma nova
- Defina um **sub-rede delegada** apropriada
- Habilite o **acesso público**, se necessário (atenção à segurança)

### 5. Outras configurações (opcional)

- Tags: adicione tags para organização e gerenciamento de custos
- Backup, segurança, manutenção e diagnóstico podem ser configurados conforme necessidade

### 6. Revisar e criar

- Revise todas as configurações
- Clique em **"Criar"** para iniciar a implantação

> ⚠️ A criação da instância pode levar cerca de 30 minutos.

## Acessar a instância após criada

1. Vá até **Instâncias do Azure SQL** no portal
2. Selecione a instância criada
3. Use o nome do host fornecido para conectar-se via SQL Server Management Studio (SSMS) ou outras ferramentas compatíveis

## Recursos adicionais

- [Documentação oficial da Microsoft](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/instance-create-quickstart?view=azuresql&tabs=azure-portal)
- [Documentação do SQL Server Management Studio (SSMS)](https://learn.microsoft.com/pt-br/sql/ssms/download-sql-server-management-studio-ssms)

---

## Licença

Este projeto segue os termos de uso da sua assinatura do Azure. Consulte as políticas da Microsoft para mais detalhes.
