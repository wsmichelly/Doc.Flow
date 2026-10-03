# Doc.Flow
Sistema web para tramitação e gestão documental pública/corporativa. Inclui engenharia de software, modelagem relacional 3FN, diagramas UML, protótipo Figma e script SQL.

> **Status do Projeto:** *Em Desenvolvimento (Fase de Engenharia de Software e Modelagem concluídas; codificação da interface/API em andamento).*

---

## O Projeto

O **Doc.Flow** é uma solução web projetada para automatizar, organizar e auditar a tramitação de documentos e processos administrativos na gestão pública e corporativa. 

O sistema substitui fluxos manuais por um processo digital rastreável, gerando comprovantes de protocolo, controle de prazos e níveis de acesso restritos para garantir conformidade e transparência.

---

## Tecnologias e Arquitetura

- **Arquitetura:** MVC (Model-View-Controller)
- **Modelagem de Dados:** Banco de Dados Relacional normalizado até a **3ª Forma Normal (3FN)**
- **Linguagem de Banco de Dados:** SQL (MySQL)
- **Modelagem de Sistemas:** UML (Casos de Uso, Diagrama de Classes e Diagrama de Atividades)
- **Prototipação & UI/UX:** Figma
- **Stack Planejada para Implementação:**
  - **Front-end:** HTML5, CSS3, JavaScript
  - **Back-end:** Java
  - **SGBD:** MySQL

---

##  Engenharia de Software e Artefatos de Projeto

A fase inicial do projeto focou no levantamento de requisitos, regras de negócio e estruturação lógica da aplicação:

### 1. Requisitos e Regras de Negócio
- **Perfil Solicitante (Cidadão) vs. Analista:** Controle hierárquico de acesso e permissões.
- **Motor de Tramitação:** Atualização automática de status (*Pendente*, *Em Análise*, *Deferido/Indeferido*).
- **Trilha de Auditoria:** Histórico detalhado de movimentação com registro de ações e responsáveis.

### 2. Diagramas UML
- **Diagrama de Classes:** Estrutura lógica com herança da classe `Usuário`, centralidade da entidade `Protocolo` e validação por hash/logs.
- **Diagrama de Atividades:** Mapeamento do fluxo de decisão, triagem e prazos do analista.

### 3. Modelagem de Banco de Dados (3FN)
- **Modelo Conceitual (MER) e Lógico:** Estrutura relacional conectando `CIDADÃO`, `PROTOCOLO`, `DOCUMENTO`, `ANALISTA`, `DEPARTAMENTO` e `HISTÓRICO_TRAMITAÇÃO`.
- **Script SQL:** Disponível no repositório na pasta `/database` (criação de tabelas, relacionamentos e dados de teste).

---

## Protótipo da Interface (UI/UX)

Telas desenvolvidas no Figma focadas em usabilidade e estilo Kanban modular:

- **Quadro Geral do Analista:** Gestão por colunas (*Novos Protocolos*, *Em Análise*, *Finalizados*).
- **Detalhes do Protocolo:** Centralização dos dados do requerente, visualizador de anexos e ações rápidas (*Aprovar*, *Reprovar*, *Solicitar Complemento*).

*(Dica: se quiser, você pode colar links das imagens ou GIFs do Figma aqui)*

---

##  Roadmap de Desenvolvimento

- [x] Levantamento de Requisitos Funcionais e Não Funcionais
- [x] Diagramação UML (Casos de Uso, Classes, Atividades)
- [x] Modelagem de Banco de Dados (MER, Lógico e Script SQL 3FN)
- [x] Prototipação de Alta Fidelidade no Figma
- [ ] Criação do Banco de Dados local/nuvem
- [ ] Construção do Front-end (HTML/CSS/JS)
- [ ] Desenvolvimento da API e integração com banco de dados
- [ ] Testes de integração e fluxo completo

---

## Autores
- Michelly Rodrigues Silva 
- Ryan Matheus Duran
- Pedro Henrique Rodrigues


Trabalho desenvolvido no curso de **Análise e Desenvolvimento de Sistemas (CEUNSP)**.
