# Roadmap Matricial

### TRIBE DSM-4 (WEB) - SQUAD 4

## Visão Geral

Este projeto visa desenvolver um sistema completo de gerenciamento de classes, incluindo administração de alunos, professores, matrículas, chamadas, digitação de notas e um dashboard de desempenho escolar.

## Participantes

- **Product Owner (P.O.):** Asher
- **Squad Matricial:** Renato Hioji (DevOps), Gustavo Kawamoto (QA), Ana Pupo e Nicolle (UX),Rodrigo(Data Science)

## Tecnologias Utilizadas

- **Servidores:** Debian
- **Banco de Dados:** PostgreSQL
- **Ferramenta de Prototipação e Pesquisa:** Figma
- **CI/CD & Automação:** GitHub Actions
- **Versionamento de Código:** Git
- **Padrões de Código:** Definidos pelo QA e implementados pela equipe de desenvolvimento terceirizada

## Funções Principais

- **Alunos**
- **Professores**
- **Cursos**
- **Turmas**
- **Matrículas**
- **Chamada**
- **Digitação de Notas**
- **Boletim**
- **Dashboard de Desempenho Escolar**

## Roadmap

### Sprint 1: Setup Inicial e Definições Iniciais de UX

**Duração:** 1 - semana
**Período:** 02/09 - 08/09

- **Objetivo:**

  - Configurar o ambiente de desenvolvimento no servidor Debian e configurar CI/CD.
  - Definir fluxos principais de usuários e wireframes iniciais no Figma.
  - Estabelecer padrões de código e boas práticas para a equipe de desenvolvimento terceirizada (QA).

- **Tarefas:**
  - Setup de servidor com Debian e PostgreSQL (DevOps)
  - Configuração de pipelines CI/CD para automação (DevOps)
  - Criação de wireframes para as telas de cadastro de Alunos e Professores no Figma (UX)
  - Documentação de padrões de código e testes (QA)
  - Integração com a equipe de desenvolvimento terceirizada para começar a implementação (Todos)
  - Configuração inicial do banco de dados PostgreSQL, definição de políticas de backup e criação de índices e constraints iniciais. (Data Science)

### Sprint 2: Definição e Pesquisa de UX para Cursos e Turmas

**Duração:** 1 semana  
**Período:** 09/09 - 15/09

- **Objetivo:**

  - Realizar pesquisa de UX para cursos e turmas, e definir protótipos no Figma.
  - QA garante que os padrões de código estão sendo seguidos e que o banco de dados PostgreSQL está configurado corretamente.

- **Tarefas:**
  - Definição de telas e fluxos de Cursos e Turmas no Figma (UX)
  - Garantir a configuração adequada de PostgreSQL e otimização de queries (DevOps)
  - Validação de código e integração com desenvolvedores (QA)
  - Validação do modelo de dados para Cursos e Turmas, ajuste de índices e otimização de queries SQL conforme novas necessidades. (Data Science)

### Sprint 3: Validação de Matrículas e

**Duração:** 1 semana  
**Período:** 16/09 - 22/09

- **Objetivo:**

  - UX ajusta fluxos de matrículas e chamadas com base em feedback e pesquisas.
  - QA faz revisão de código e testes automatizados para garantir a qualidade do código entregue.

- **Tarefas:**
  - Atualização de protótipos no Figma (UX)
  - Automação de testes para Matrículas e Chamada no pipeline CI/CD (DevOps)
  - Validação de código e integração com PostgreSQL (QA)
  - Ajustes no banco de dados para Matrículas e Chamada, análise de performance das queries e monitoramento da saúde do banco de dados. (Data Science)

### Sprint 4: Digitação de Notas e Geração de Boletim

**Duração:** 1 semana  
**Período:** 23/09 - 29/09

- **Objetivo:**

  - UX projeta a experiência de digitação de notas e geração de boletim no Figma.
  - QA valida código e padrões para essas novas funcionalidades, garantindo a integração contínua no ambiente Debian/PostgreSQL.

- **Tarefas:**
  - Prototipagem no Figma para Notas e Boletim (UX)
  - Configuração de testes automatizados para Notas e Boletim no CI/CD (DevOps)
  - Validação de código e padrões de segurança para banco de dados (QA)
  - Ajustes no modelo de dados para Notas e Boletim, implementação de triggers e stored procedures, além de testes de carga para o banco de dados. (Data Science)

### Sprint 5: Design e Validação do Dashboard de Desempenho Escolar

**Duração:** 1 semana  
**Período:** 30/09 - 06/10

- **Objetivo:**

  - UX finaliza o design do dashboard no Figma.
  - QA garante que os gráficos e consultas SQL no PostgreSQL estejam otimizados e dentro dos padrões estabelecidos.

- **Tarefas:**
  - Prototipagem e design do Dashboard no Figma (UX)
  - Implementação de testes de performance e integração contínua para o Dashboard (DevOps)
  - Validação de código e queries SQL otimizadas para o Dashboard (QA)
  - Otimização das queries SQL para o Dashboard, implementação de índices adequados e verificação de segurança e performance no banco de dados.(Data Science)

### Sprint 6: Otimização e Garantia de Qualidade

**Duração:** 1 semana  
**Período:** 07/10 - 13/10

- **Objetivo:**

  - Revisão e otimização geral do sistema para garantir desempenho e usabilidade.
  - Garantir a segurança e a estabilidade do servidor Debian e PostgreSQL.

- **Tarefas:**
  - Revisão de UX com base em feedback e ajustamentos no Figma (UX)
  - Implementação de testes de stress e segurança no servidor e banco de dados (DevOps)
  - Testes finais de código e QA (QA)
  - Auditoria completa do banco de dados para ajustes de performance e segurança, incluindo revisão de políticas de backup e failover. (Data Science)

### Sprint 7: Integrações com APIs Externas

**Duração:** 1 semana  
**Período:** 21/10 - 27/10

- **Objetivo:**

  - Implementar integrações com sistemas externos (ex.: APIs de pagamento ou autenticação) e garantir que o servidor Debian e o PostgreSQL suportem essas integrações com segurança.

- **Tarefas:**
  - Ajustes de design no Figma para suportar integrações (UX)
  - Configuração de pipelines para APIs e testes de integração (DevOps)
  - Validação de segurança e padrões de código nas integrações (QA)
  - Ajustes na arquitetura do banco de dados para suporte a integrações externas, garantindo segurança e performance.(Data Science)

### Sprint 8: Conclusão e Refinamento Final

**Duração:** 1 semana  
**Período:** 28/10 - 03/11

- **Objetivo:**

  - Refinamento final das funcionalidades, correção de bugs e ajustes finais de usabilidade e lógica de negócios.

- **Tarefas:**
  - Revisão final de UX e design no Figma (UX)
  - Testes finais de regressão e performance no ambiente Debian/PostgreSQL (DevOps)
  - Revisão final de código e qualidade (QA)
  - Tuning final no banco de dados, documentação de estrutura e otimizações, além da participação nas validações finais.(Data Science)

## Considerações Finais

A squad matricial focará em garantir a qualidade, performance e segurança do sistema, utilizando Debian como servidor, PostgreSQL para banco de dados e Figma para as pesquisas de UX e prototipagem. A validação rigorosa será conduzida pelo QA para garantir que o código entregue pelos desenvolvedores terceirizados atenda aos padrões estabelecidos.
