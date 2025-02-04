<<<<<<< HEAD
# Cadastro Central de Usuários para Municípios

## Estrutura de Trabalho

### Branches do GitHub

#### Branches Principais:
- **main**: Código em produção.
- **development**: Ambiente de integração para funcionalidades e correções.
- **staging**: Ambiente de teste antes do deploy final.

#### Branches de Trabalho:
- Funcionalidade nova: `feature/nomefuncionalidade-cardgerador`.
- Bug não emergencial: `bugfix/nomedobug-cardgerador`.
- Bug emergencial: `hotfix/nomedobug-cardgerador`.

### Fluxo de Merge
1. Merge inicial para `development`.
2. Testes e validações na branch `staging`.
3. Aprovação do PO e do cliente.
4. Merge final para `main`.

### Regras de Qualidade
- Branches `development`, `staging` e `main` devem ser espelhadas.
- Proibição de merge direto em `main`.
- CI/CD configurado para garantir que apenas códigos testados e aprovados avancem.

### Práticas de Versionamento e Tags

#### Versionamento Semântico (SemVer):
- `v1.0.0`: Versão principal com funcionalidade inicial.
- `v1.1.0`: Adição de novas funcionalidades.
- `v1.1.1`: Correção de bugs menores.

#### Uso de Tags:
- Tags serão criadas em merges para `main`, facilitando rastreabilidade no histórico do projeto.

## Automatização com CI/CD

### Pipeline CI (Integrado com GitHub Actions):
- Rodar testes automatizados.
- Garantir que commits estejam em conformidade com padrões.

### Pipeline CD:
- Deploy automatizado para `staging` após aprovação.
- Deploy para produção após validações finais.

## Gerenciamento de Atividades e Correções

### Fluxo de Trabalho para Correção de Bugs e Novas Atividades

#### Correção Isolada na Branch `bugfix` ou `hotfix`:
- Branches para correção de bugs são criadas a partir de `staging` ou `main`.
- Exemplos:
  - `bugfix/corrigir-filtro-card123` (bug não emergencial).
  - `hotfix/corrigir-filtro-card123` (bug emergencial).
- Correções são testadas e validadas antes do merge.

#### Prioridade e Planejamento do Bug:
- **Alta prioridade**: Resolve-se na sprint atual.
- **Baixa prioridade**: Entra no backlog para a próxima sprint.

#### Novas Atividades Seguem Normalmente em `feature/`:
- Novas atividades são criadas em branches como `feature/nova-funcionalidade-cardX`, baseadas em `development`.

#### Evitar Conflitos com `bugfix`:
- Antes do merge de uma branch `bugfix`, atualize-a com as mudanças mais recentes de `development`.
- Resolva conflitos localmente antes do merge final.

## Cronograma de Atividades

### 06/01/2025 - Apresentação do Projeto e Arquitetura Limpa
**Teoria (Segunda-feira):**
- Apresentação do problema: Cadastro Central de Usuários para municípios.
- Introdução à Arquitetura Limpa: princípios, camadas e benefícios.
- Discussão sobre modularização e organização do projeto.
- Debate sobre a divisão do projeto em microsserviços, considerando os quatro grupos e suas linguagens escolhidas.
- Escolha dos grupos por Linguagem de aderência.
- Explicação da forma de trabalho com GitHub.
- Atividade prática: Esboçar o modelo inicial do projeto, identificando as entidades principais, responsabilidades das camadas e principais módulos.

### 08/01/2025 - Modelagem e UML
**Laboratório (Quarta-feira):**
- Introdução à modelagem UML: diagramas de classes e objetos.
- Criação de um diagrama inicial para representar um cadastro simplificado.
- Ferramentas sugeridas: Draw.io.

### 13/01/2025 - Linguagem de Programação e Estruturas Básicas
**Teoria (Segunda-feira):**
- Aprofundamento em abstração de dados.
- Modificadores de visibilidade (protegido, privado, público): quando e por que usar.
- Tarefa prática: Implementar exemplos de visibilidade e demonstrar seu impacto na segurança e modularidade.

### 15/01/2025 - Abstração de Dados e Modularização
**Laboratório (Quarta-feira):**
- Criar módulos para separar funcionalidades (ex.: módulo para usuários e outro para autenticação).
- Implementar a visibilidade de atributos e métodos.

### 20/01/2025 - Relacionamentos entre Classes
**Teoria (Segunda-feira):**
- Hierarquias: generalização/especialização e agregação.
- Enumerações e classes internas.
- Relacionamentos entre classes: associação, agregação, composição.
- Modularização: organização e separação de responsabilidades.
- Interfaces vs. Classes Abstratas: como, quando e por que utilizar.
- Tarefa prática: Criar um relacionamento entre classes (ex.: classe "Município" e classe "Usuário").

### 22/01/2025 - Herança e Polimorfismo
**Laboratório (Quarta-feira):**
- Implementar herança entre classes (ex.: "Pessoa Física" e "Pessoa Jurídica").
- Demonstrar polimorfismo com métodos redefinidos.

### 27/01/2025 - Tratamento de Exceções
**Teoria (Segunda-feira):**
- Hierarquia de exceções.
- Como capturar e lançar exceções.
- Introdução ao Stack Trace: como interpretá-lo e utilizá-lo para depuração.
- Tarefa prática: Implementar tratamento de erros no cadastro (ex.: CPF inválido).

### 29/01/2025 - Arquivos e Persistência
**Laboratório (Quarta-feira):**
- Implementar leitura e escrita de arquivos textuais.
- Salvar e carregar o cadastro de usuários.

### 03/02/2025 - Coleções Genéricas
**Teoria (Segunda-feira):**
- Estruturas de dados genéricas (listas, mapas).
- Manipulação de coleções para armazenar usuários.
- Tarefa prática: Substituir arrays por listas genéricas na aplicação.

### 05/02/2025 - Padrões de Projeto
**Laboratório (Quarta-feira):**
- Introdução a padrões como Singleton e Factory.
- Implementar pelo menos um padrão no projeto.

### 10/02/2025 - Revisão Geral
**Teoria (Segunda-feira):**
- Análise crítica do que foi desenvolvido.
- Identificar pontos de melhoria.
- Tarefa prática: Finalizar funcionalidades pendentes.

### 12/02/2025 - Apresentação Final
**Entrega (Quarta-feira):**
- Apresentação do projeto por equipes.
- Discussão dos desafios enfrentados e soluções implementadas.
=======
Trabalho da Disciplina: Orientação a Objetos

Apresentação

Este repositório contém o trabalho desenvolvido para a disciplina de Orientação a Objetos. O projeto foi elaborado com base nos princípios fundamentais da programação orientada a objetos, incluindo encapsulamento, herança, polimorfismo e abstração.

O objetivo deste trabalho é demonstrar a aplicação desses conceitos através de uma solução prática e funcional, utilizando uma linguagem de programação orientada a objetos.

Lista de Participantes

Abaixo, preencha os nomes dos participantes do trabalho:

Usuário: PaulaSuyaneDEV   ---  Aluno: Paula Suyane 

Usuário: jaoxavier        ---  Aluno: João Victor Xavier Lima  

Usuário: ferreiraitalvar  ---  Aluno: Italvar Ferreira

Usuário: Igortpfalcao     ---  Aluno: igor Teixeira Passos Falcão  

Usuário: tailasnakin e loureorganic --- Aluno: Taila da Silva Santos

Usuário: shenioalves ---  Aluno:  Shenio de Souza Alves

Usuário:  Scoppetta  Aluno:  Henrique Queiroz Scoppetta Sampaio

Usuário:  PeuMAndrade  Aluno: Pedro Henrique Andrade  
Usuário:  ---  Aluno:  
Usuário:  ---  Aluno:  
Usuário:  ---  Aluno:  
Usuário:  ---  Aluno:  
Usuário:  ---  Aluno:  
Usuário:  ---  Aluno:  
Usuário:  ---  Aluno:  
Usuário:  ---  Aluno:  
Usuário:  ---  Aluno:  



























































>>>>>>> upstream/main
