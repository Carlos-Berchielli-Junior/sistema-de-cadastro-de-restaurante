# 🍽️ Sabor Express — CLI Restaurant Management System

[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

O **Sabor Express** é uma aplicação interativa em linha de comando (CLI) desenvolvida em Python para o gerenciamento dinâmico de restaurantes. O sistema permite o cadastro de novos estabelecimentos, categorização, listagem formatada e alternância do estado de atividade, simulando o ecossistema de operação interna de uma plataforma de delivery.

---

## 📌 Índice
- [Funcionalidades](#-funcionalidades)
- [Arquitetura e Fluxo do Sistema](#-arquitetura-e-fluxo-do-sistema)
- [Conceitos Técnicos Aplicados](#-conceitos-técnicos-aplicados)
- [Como Executar o Projeto](#-como-executar-o-projeto)
- [Melhorias Futuras](#-melhorias-futuras)
- [Licença](#-licença)

---

## 🚀 Funcionalidades

1. **Menu Interativo (CLI):** Interface limpa no terminal com navegação guiada por entrada numérica.
2. **Cadastro de Restaurantes:** Permite a inserção de novos estabelecimentos definindo nome e categoria gastronômica. Por padrão, novos registros iniciam como `Desativados`.
3. **Listagem Formatada:** Exibição dos dados tabulados utilizando espaçamento dinâmico (`ljust`) para garantir a legibilidade das colunas no terminal.
4. **Alternância de Estado:** Ativa ou desativa um restaurante dinamicamente através de busca por correspondência de string.
5. **Resiliência a Falhas:** Sistema blindado contra quebras de execução caso o usuário insira caracteres inválidos em menus numéricos.

---

## 💻 Conceitos Técnicos Aplicados

* **Estruturas de Dados Compostas:** Utilização de uma lista global contendo dicionários (`List[Dict[str, Any]]`) para modelar a entidade do restaurante e simular a persistência de dados em memória.
* **Modularidade e Clean Code:** Código totalmente fatiado em funções com responsabilidade única (*Single Responsibility Principle*), facilitando a manutenção e legibilidade.
* **Documentação (Docstrings):** Todas as funções contêm documentação interna no padrão PEP 257 para detalhar comportamentos, entradas e saídas.
* **Tratamento de Exceções:** Implementação de blocos `try/except` capturando `ValueError` para mitigar comportamentos inesperados em entradas do teclado.
* **Expressões Condicionais Inline:** Uso do operador ternário do Python para simplificar atribuições de strings (*Ex: `Ativado if ... else Desativado`*).

---
