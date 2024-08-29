# 🚀 Lançador Automático para o Fiscal Varejo do EFD Contribuições

## 📋 Descrição do Projeto

Este projeto implementa um módulo backend para automatizar o lançamento de informações fiscais de vendas no varejo para o **EFD Contribuições**, parte do **SPED** (Sistema Público de Escrituração Digital). O módulo realiza as seguintes etapas:

- Coleta automáticamente de uma tela as informações necessárias para cada Lançamento.
- Adiciona corretamente os Lançamentos solicitados como: Energia, Depreciação, Aluguel e etc.
- Confirmação dos lançamentos.
- Criação de novo TXT para importação na ferramenta EFD Contribuições.

## 📁 Estrutura do Projeto

├── docs/
│   ├── casos_de_uso.pdf
│   ├── diagramas_de_sequencia.pdf
│   └── diagramas_de_classe.pdf
├── src/
│   ├── controllers/
│   ├── models/
│   ├── services/
│   ├── routes/
│   └── app.ts
├── tsconfig.json
├── package.json
└── README.md

## ✅ Requisitos

### Requisitos Funcionais

- **Coleta de Dados**: Captura automática dos Lançamentos.
- **Processamento de Dados**: Validação e formatação dos dados conforme normas da Receita Federal.
- **Geração de Arquivos**: Criação de arquivos EFD Contribuições compatíveis com versão atualizada.
- **Notificação de Erros**: Alertas em caso de falhas na coleta, processamento ou envio dos dados.

### Requisitos Não Funcionais

- **Performance**: Processamento e geração de arquivos em até 5 Minutos após informações passadas.
- **Escalabilidade**: Suporte para até Diversas Lojas no Sistema de Lucro Real.
- **Conformidade**: Alinhamento com as leis e regulamentações fiscais vigentes.
- **Disponibilidade**: Uptime mínimo de 99,9%.

### Regras de Negócio

- **Validação Fiscal**: Somente lançamentos conformes devem ser solicitadas.
- **Correção de Erros**: Possibilidade de correção manual dos dados antes da criação do novo arqu.

### Requisitos de Usuário

- **Interface de Usuário**: Acesso a relatórios e status de envio.
- **Arquivo Compativel**: Arquivo com necessidade de conter versão mais atualizada do Sped Contribuições.

### Requisitos de Sistema

- **Integração**: Arquivo contendo as informações necessárias para o lançamento correto.
- **Tecnologias**: Desenvolvimento em TypeScript com Node.js e Express.js, utilizando PostgreSQL.

## 🔍 Análise de Viabilidade

### Tecnologias Utilizadas

- **Linguagem**: TypeScript - Segurança e escalabilidade.
- **Framework**: Express.js - Simplicidade e eficiência.
- **Banco de Dados**: PostgreSQL - Confiabilidade e robustez.

### Infraestrutura

- **Arquivos Corretos**: Garantia de alta confiança e perfeição nos lançamentos.
- **Segurança**: Implementação de SSL/TLS para proteção de dados.

### Padrões de Projeto

- **MVC (Model-View-Controller)**: Estruturação do código.
- **Padrão de Repositório**: Acesso organizado aos dados.

## 🎯 Priorização dos Requisitos

### Técnica MoSCoW

- **Must Have**: Coleta de Dados, Processamento de Dados, Geração de Arquivos.
- **Should Have**: Interface de Usuário, Arquivo Compativel.
- **Could Have**: Notificação de Erros, Correção de Erros.
- **Won’t Have**: Funcionalidades avançadas de análise de Lançamentos.

## 📊 Modelos de Utilização

  Sistema de Lançamento Automático EFD --> Usuário/Dados - Coleta de Dados --> Processamento ou Edição dos Lançamentos -->
  Gerar Arquivo TXT --> Validação Arquivo --> Transmissão a Receita Federal ou Envio aos Advogados
