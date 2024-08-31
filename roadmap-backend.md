# Roadmap Back-End - API REST em Node.js
### 31 de agosto, 2024
### TRIBE DSM-4 (WEB) - SQUAD 3: Vinícius Gabriel Miranda Gomes (PO)
#### Equipe: Especialistas em desenvolvimento back-end (Node.js)
* Ana Cristina Domingues
* Eliharison Gonçalves Sabino Gabriel
* Matheus da Silva Moura
* Victor Luis Camargo de Aguiar
* Vinicius Leal Alves
* Guilherme Miyamoto 

#### Stacks:
* Node.js
* TypeScript
* Express
* Sequelize

#### Story User:
* Alunos
* Professores
* Cursos
* Turmas
* Matrículas
* Chamada
* Digitação de Notas
* Boletim
* Dashboard de desempenho escolar

#### Níveis de acesso:
1. Aluno
2. Professor
3. Secretaria e administrador

### Sprint 1: Configuração Inicial
#### Duração: 1 semana
#### Período: 02/09 - 08/09
**Tarefas:**
+ Instalação e configuração do ambiente de desenvolvimento com TypeScript.
+ Configuração de scripts no package.json para desenvolvimento com ts-node e produção.
+ Instalação e configuração de dependências principais e de desenvolvimento.
+ Configuração inicial do servidor Express básico.
+ Criação de estrutura básica de pastas e arquivos para o projeto.
+ Documentação dos padrões de código e projeto.
+ Estabelecimento de conexão com o banco de dados usando Sequelize.

#### Entregáveis:
- Ambiente de desenvolvimento configurado.
- Estrutura inicial do projeto definida.

### Sprint 2: Modelagem de Dados
#### Duração: 1 semana
#### Período: 09/09 - 15/09
**Tarefas:**
+ Configuração do banco de dados e criação de variáveis de ambiente.
+ Modelagem de dados e criação de modelos para as entidades: Aluno, Professor, Curso, Turma, Matrícula, Nota.
+ Documentação da arquitetura de dados e modelo de entidades.
#### Entregáveis:
- Banco de dados configurado e conectado.
- Modelos criados para as entidades principais.

### Sprint 3: Implementação de Funcionalidades CRUD (Parte 1)
#### Duração: 1 semana
#### Período: 16/09 - 22/09
**Tarefas:**
1. CRUD para Alunos:
+ Criar rotas para operações CRUD (criação, leitura, atualização e exclusão) para Alunos.
+ Implementar controladores para gerenciar as operações CRUD de Alunos.
+ Definir validações de entrada de dados para Alunos (e.g., matrícula, nome, data de nascimento).
2. CRUD para Professores:
+ Criar rotas para operações CRUD para Professores.
+ Implementar controladores para gerenciar as operações CRUD de Professores.
+ Definir validações de entrada de dados para Professores (e.g., matrícula, nome, especialidade).
3. CRUD para Cursos:
+ Criar rotas para operações CRUD para Cursos.
+ Implementar controladores para gerenciar as operações CRUD de Cursos.
+ Definir validações de entrada de dados para Cursos (e.g., código do curso, nome, carga horária).
4. CRUD para Matrículas:
+ Criar rotas para operações CRUD para Matrículas.
+ Implementar controladores para gerenciar as operações CRUD de Matrículas.
+ Definir validações de entrada de dados para Matrículas (e.g., aluno, turma, data de matrícula).
5. Testes:
+ Revisão e testes básicos das funcionalidades CRUD de Aluno e Professor
+ Documentar a API para as rotas de Alunos e Professores.
#### Entregáveis:
- Operações CRUD para entidades Alunos, Professores, Cursos e Matrículas

### Sprint 4: Implementação de Funcionalidades CRUD (Parte 2)
#### Duração: 1 semana
#### Período: 23/09 - 29/09
**Tarefas:**
1. CRUD para Turmas:
+ Criar rotas para operações CRUD para Turmas.
+ Implementar controladores para gerenciar as operações CRUD de Turmas.
+ Definir validações de entrada de dados para Turmas (e.g., código da turma, período, professor responsável).
2. CRUD para Chamada:
+ Criar rotas para operações CRUD para Chamada.
+ Implementar controladores para gerenciar as operações CRUD de Chamada.
+ Definir validações de entrada de dados para Chamada (e.g., data, turma, presença de alunos).
3. CRUD para Digitação de Notas:
+ Criar rotas para digitação e atualização de notas.
+ Implementar controladores para gerenciar a digitação de notas.
+ Definir validações de entrada de dados para notas (e.g., aluno, turma, nota, tipo de avaliação).
4. CRUD para Boletim:
Criar rotas para geração e visualização de boletins.
+ Implementar controladores para gerar boletins com base nas notas digitadas.
+ Definir regras de negócio para o cálculo de médias e geração de boletins.
5. Documentação e Testes:
+ Documentar a API para as rotas de Cursos, Turmas, e Matrículas.
+ Desenvolver testes unitários e de integração para as operações CRUD de Cursos, Turmas, e Matrículas.
#### Entregáveis:
- Operações CRUD para entidades Turmas, Chamadas, Digitação de Notas e Boletim

### Sprint 5: Autenticação e Autorização
#### Duração: 1 semana
#### Período: 30/09 - 06/10
**Tarefas:**
+ Implementação de autenticação de usuário usando JWT (token).
+ Criação de rotas de autenticação (login e cadastro) com diferentes níveis de acesso (admin, professor, aluno).
+ Desenvolvimento de middlewares de autenticação para verificar o token JWT em rotas protegidas.
+ Documentação da implementação de autenticação e autorização.
+ Testes de fluxos de autenticação e autorização.
*+Permissões de Acesso:*
+ Definir permissões de acesso para alunos (visualizar apenas seus próprios dados).
+ Definir permissões de acesso para professores (visualizar e editar seus próprios dados, visualizar dados de alunos, visualizar matrículas e turmas).
+ Definir permissões de acesso para secretaria e administradores (acesso completo aos dados de Alunos e Professores, criar e gerenciar cursos, turmas e matrículas).
+ Configurar permissões para acesso a notas e chamadas: professores (digitação e visualização), alunos (visualização de seu próprio boletim e presença), secretaria e administradores (gerenciamento completo).
#### Entregáveis:
+ Sistema de autenticação com JWT implementado.
- Autorização baseada em níveis de acesso.

### Sprint 6: Validações e Tratamento de Erros
#### Duração: 1 semana
#### Período: 07/10 - 13/10
**Tarefas:**
+ Implementação de validações de entrada de dados para todas as entidades. 
+ Desenvolvimento de middlewares de tratamento de erros globais.
+ Refatoração de código para inclusão de validações e tratamento de erros.
+ Testes de validação e tratamento de erros.
#### Entregáveis:
- Validações de entrada de dados implementadas.
- Tratamento de erros configurado.

### Sprint 7: Testes, Correções finais e Finalizar Documentação
#### Duração: 1 semana
#### Período: 21/10 - 27/10
**Tarefas:**
+ Escrita de testes unitários para rotas e controladores de todas as entidades.
+ Revisão de testes e cobertura de código.
+ Documentação com Swagger.
#### Entregáveis:
- Testes unitários para todas as rotas e controladores.
- Documentação inicial com Swagger criada.
- Feedbacks coletados e ajustes realizados.
- API finalizada e online
