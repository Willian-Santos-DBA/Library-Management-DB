# 📚 Library Management System: Modelagem e Implementação SQL

Este repositório contém a solução completa para o estudo de caso de um sistema de gerenciamento de biblioteca universitária. O projeto abrange desde o levantamento de requisitos e modelagem de dados até a implementação prática utilizando SQL.

## 💻 Sobre o Projeto
O objetivo é gerenciar o acervo de livros, autores, categorias de obras e o fluxo de empréstimos (locações) para usuários da instituição. O projeto foi dividido em duas fases:
1. **Design de Arquitetura:** Criação dos modelos Conceitual e Lógico.
2. **Engenharia de Dados:** Normalização, criação de scripts DDL (estrutura) e DML (dados e consultas).

## 🛠️ Tecnologias e Ferramentas
- **Modelagem:** brModelo Web.
- **Banco de Dados:** MySQL / PostgreSQL.
- **Linguagem:** SQL (Structured Query Language).

---

## 📐 Fase 1: Modelagem de Dados

Nesta etapa, as regras de negócio foram mapeadas para identificar entidades, atributos e relacionamentos:
- **Relação Muitos-para-Muitos (N:M):** Implementada entre Livros e Autores.
- **Relação Um-para-Muitos (1:N):** Aplicada entre Categorias e Livros, e entre Usuários e Locações.

*(Os diagramas Conceitual e Lógico estão disponíveis nos arquivos deste repositório).*

---

## ⚙️ Fase 2: Implementação e Normalização

### 1. Normalização
O modelo foi revisado para garantir a integridade referencial e eliminar redundâncias, aplicando as Formas Normais:
- **1FN:** Garantia de atomicidade dos dados.
- **2FN e 3FN:** Eliminação de dependências parciais e transitivas, garantindo que cada atributo não-chave dependa exclusivamente da chave primária.

### 2. Implementação SQL (Scripts)
O script SQL contido neste repositório executa as seguintes operações:
- **DDL (Data Definition Language):** Criação de tabelas com definição de Primary Keys, Foreign Keys e tipos de dados otimizados.
- **DML (Data Manipulation Language):** Inserção de registros de teste para validação das restrições de integridade.
- **Queries de Negócio:** Listagem de usuários e consultas filtradas por categorias usando comandos `SELECT` e `INNER JOIN`.

---
*Desenvolvido por: Willian Nunes dos Santos.*
