# 🏥 ConsultaVAG - Sistema de Regulação Ambulatorial

![Status](https://img.shields.io/badge/Status-Análise_e_Projeto-blue) ![Metodologia](https://img.shields.io/badge/Metodologia-RUP-orange) ![Instituição](https://img.shields.io/badge/Instituição-UPE-red)

## 📋 Sobre o Projeto

O **ConsultaVAG** é um sistema digital projetado para substituir o processo manual de regulação ambulatorial da **Secretaria Estadual de Saúde (SES)**.

Atualmente, o processo depende de planilhas para o gerenciamento de cotas e distribuição regional, o que gera filas extensas e falta de visibilidade. O ConsultaVAG visa centralizar essas informações, permitindo que as **12 GERES (Gerências Regionais de Saúde)** e os municípios gerenciem suas cotas, filas de espera (demanda reprimida) e agendamentos de forma transparente e eficiente.

## 🏛️ Arquitetura do Sistema

O projeto segue uma arquitetura em camadas baseada no **RUP (Rational Unified Process)**, garantindo a separação de responsabilidades e facilitando a manutenção:

1.  **Camada de Apresentação (View):** Responsável pela interação com o usuário (Boundaries).
2.  **Camada de Aplicação (Controller):** Orquestra os casos de uso e regras de aplicação.
3.  **Camada de Domínio (Model):** Contém as entidades de negócio (ex: Cota, Paciente, Demanda).
4.  **Camada de Infraestrutura:** Repositórios e acesso a dados.

## 📝 Artefatos Produzidos

A documentação do projeto está consolidada nos seguintes ficheiros:

### 1. Especificação de Requisitos (`APS - Consulta Vag.pdf`)
Este documento atua como a base do projeto, contendo:
* **Visão Geral:** Definição do problema de regulação ambulatorial e objetivos do sistema.
* **Requisitos:** Lista completa de Requisitos Funcionais (RF) e Não-Funcionais (RNF).
* **Regras de Negócio:** Normas da SES para distribuição e remanejamento de cotas.
* **Especificação de Casos de Uso:** Detalhamento textual dos fluxos e cenários.

### 2. Análise do Sistema (`Doc.Analise-Consulta Vag.pdf`)
Focado na modelagem inicial e compreensão do problema:
* **Diagramas de Classes de Análise:** Estrutura preliminar das classes (Boundary, Control, Entity).
* **Diagramas de Sequência de Análise:** Interações iniciais entre os objetos do sistema.

### 3. Projeto de Software (`Doc.Projeto_ConsultaVAG.pdf`)
Detalhamento técnico para implementação (Arquitetura RUP):
* **Arquitetura:** Visão lógica das camadas (Apresentação, Aplicação, Domínio, Infraestrutura).
* **Diagramas de Classes de Projeto:** Estrutura refinada com assinaturas de métodos.
* **Diagramas de Sequência de Projeto:** Detalhamento técnico das interações para casos de uso críticos (ex: *Distribuir Cotas*, *Consumir Cota*).

## 🚀 Funcionalidades Principais Projetadas

* **Gestão de Estrutura:** Cadastro de GERES, Municípios e Unidades Executantes.
* **Definição de Oferta:** A SES define a capacidade mensal de atendimento por especialidade.
* **Distribuição de Cotas:** Fluxo hierárquico (SES → GERES → Municípios).
* **Regulação e Fila:** Inserção de pacientes na fila de espera (Demanda Reprimida) quando não há cotas.
* **Remanejamento:** Transferência de cotas entre municípios ou GERES para corrigir distorções.
* **Painéis de Controle (Dashboards):** Visão estratégica para gestores Estaduais, Regionais e Municipais.

## 🛠 Ferramentas Utilizadas na Documentação

* **Modelagem UML:** Astah / Lucidchart.
* **Processo:** RUP (Rational Unified Process).
* **Edição de Texto:** Microsoft Word / Google Docs.

## 👥 Equipe de Desenvolvimento (UPE)

* **Bruno Rangel**
* **Erasmo Alves**
* **Everton Barbosa**
* **Nathália Bacalhau**
* **Sócrates Farias**

---
*Este repositório serve como a base de conhecimento técnica para a implementação futura do Sistema ConsultaVAG.*