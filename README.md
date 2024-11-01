# Plano de Desenvolvimento para Sistema de Banco de Dados de Testes de Produção

## Objetivo Geral do Projeto
Desenvolver um sistema de banco de dados escalável e seguro para armazenar dados de testes de produção de dispositivos eletrônicos, com interface interativa para os usuários, armazenamento eficiente e automação de análises.

---

## 📅 Sprints e Entregáveis

### Índice
1. [Sprint 1: Configuração do Ambiente e Estrutura Inicial do Banco de Dados](#sprint-1-configuração-do-ambiente-e-estrutura-inicial-do-banco-de-dados)
1.1. [Passos para Configuração do Ambiente com Docker](#passos-para-configuração-do-ambiente-com-docker)
1.2. [Configuração do PostgreSQL com Tabelas Básicas](#configuração-do-postgresql-com-tabelas-básicas)
2. [Sprint 2: Conexão Backend e Estrutura Básica de API (Em Andamento)](#sprint-2)
3. [Sprint 3: Interface Inicial do Usuário (Frontend Angular)](#sprint-3)
4. [Sprint 4: Implementação de Filtragem e Ordenação de Dados](#sprint-4s)
5. [Sprint 5: Segurança e Controle de Acesso](#sprint-5)
6. [Sprint 6: Automação de Análise de Dados e Relatórios](#sprint-6)
7. [Sprint 7: Testes Finais e Otimização do Sistema](#sprint-7)

---

### ✔️ Sprint 1: Configuração do Ambiente e Estrutura Inicial do Banco de Dados
**Objetivo:** Preparar a infraestrutura básica para o banco de dados e o ambiente de desenvolvimento.

- **User Stories:**
  - Como desenvolvedor, quero configurar um ambiente de desenvolvimento padronizado com Docker, para garantir consistência.
  - Como engenheiro de dados, quero definir e implementar as tabelas e relacionamentos iniciais em PostgreSQL, para que o banco de dados armazene dados estruturados.
- **Atividades:**
  - [x] Configuração do ambiente Docker.
  - [x] Configuração inicial do PostgreSQL com tabelas básicas.
- **Definição de Pronto:** Ambiente configurado com Docker e PostgreSQL inicializado com tabelas de dados de teste e primeiros relacionamentos.
  
Status: **Concluída**

---

### ⬛ Sprint 2: Conexão Backend e Estrutura Básica de API (Em Andamento)
**Objetivo:** Estabelecer a comunicação entre o banco de dados e a aplicação via API.

- **User Stories:**
  - Como desenvolvedor, quero criar uma API básica em Python para conectar com PostgreSQL, para realizar operações CRUD.
  - Como usuário, quero que a API me permita acessar e modificar registros no banco de dados.
- **Atividades:**
  - [ ] Implementação de endpoints CRUD para operações básicas de leitura e escrita.
  - [ ] Testes unitários para os endpoints principais.
- **Definição de Pronto:** API funcional com endpoints CRUD, conectada ao banco de dados PostgreSQL, com testes básicos de operação.

Status: **Em Andamento**

---

### ⬜ Sprint 3: Interface Inicial do Usuário (Frontend Angular)
**Objetivo:** Criar uma interface básica para interação com os dados do banco.

- **User Stories:**
  - Como usuário, quero visualizar registros armazenados no banco de dados em uma interface intuitiva.
  - Como usuário, quero acessar detalhes de um registro específico ao clicar na interface.
- **Atividades:**
  - [ ] Configuração do projeto Angular e integração com API.
  - [ ] Implementação de exibição de registros na interface.
- **Definição de Pronto:** Interface de usuário que exibe registros do banco de dados, com navegação funcional e design básico.

---

### ⬜ Sprint 4: Implementação de Filtragem e Ordenação de Dados
**Objetivo:** Melhorar a interface com opções de filtragem e ordenação dos registros.

- **User Stories:**
  - Como usuário, quero filtrar registros por critérios específicos, para visualizar apenas os dados relevantes.
  - Como usuário, quero ordenar os registros para facilitar a análise.
- **Atividades:**
  - [ ] Implementação de filtros e ordenação na API e no frontend.
  - [ ] Testes de filtragem e ordenação para garantir a precisão.
- **Definição de Pronto:** Filtros e ordenação implementados e funcionalidade verificada na interface.

---

### ⬜ Sprint 5: Segurança e Controle de Acesso
**Objetivo:** Assegurar que apenas usuários autorizados acessem o sistema e manipulem dados.

- **User Stories:**
  - Como usuário, quero fazer login para garantir que só pessoas autorizadas acessem o sistema.
  - Como administrador, quero definir permissões para restringir o acesso a dados e funcionalidades críticas.
- **Atividades:**
  - [ ] Implementação de autenticação e autorização (OAuth2 ou JWT).
  - [ ] Controle de acesso no backend para diferentes perfis de usuários.
- **Definição de Pronto:** Autenticação e controle de acesso implementados, com testes de segurança básicos concluídos.

---

### ⬜ Sprint 6: Automação de Análise de Dados e Relatórios
**Objetivo:** Criar scripts automáticos para análise dos dados armazenados, gerando relatórios periódicos.

- **User Stories:**
  - Como engenheiro de dados, quero automatizar a análise de dados para identificar tendências e métricas sem intervenção manual.
  - Como gerente de projeto, quero relatórios automáticos para acompanhar a qualidade e o desempenho dos dispositivos.
- **Atividades:**
  - [ ] Desenvolvimento de scripts de análise em Python para integração com o banco de dados.
  - [ ] Implementação de geração e armazenamento de relatórios.
- **Definição de Pronto:** Scripts de análise funcionando com agendamento periódico e relatórios armazenados para consulta.

---

### ⬜ Sprint 7: Testes Finais e Otimização do Sistema
**Objetivo:** Garantir que o sistema esteja otimizado para alto desempenho e pronto para a produção.

- **User Stories:**
  - Como engenheiro de dados, quero otimizar consultas e estrutura de banco de dados para suportar carga alta.
  - Como usuário final, quero que o sistema funcione de forma rápida e sem erros na produção.
- **Atividades:**
  - [ ] Testes de carga e stress no banco de dados e API.
  - [ ] Otimização de consultas e estrutura de dados.
- **Definição de Pronto:** Sistema validado com desempenho otimizado, pronto para implantação.

---

## 🔄 Status de Desenvolvimento

- [x] Sprint 1: Configuração do Ambiente e Estrutura Inicial do Banco de Dados (Concluída)
- [ ] Sprint 2: Conexão Backend e Estrutura Básica de API (Em Andamento)
- [ ] Sprint 3: Interface Inicial do Usuário (Frontend Angular)
- [ ] Sprint 4: Implementação de Filtragem e Ordenação de Dados
- [ ] Sprint 5: Segurança e Controle de Acesso
- [ ] Sprint 6: Automação de Análise de Dados e Relatórios
- [ ] Sprint 7: Testes Finais e Otimização do Sistema

---

# 1. Sprint 1: Configuração do Ambiente e Estrutura Inicial do Banco de Dados

## User Stories
1. **Como desenvolvedor**, quero configurar um ambiente de desenvolvimento padronizado com Docker, para garantir consistência entre as etapas de desenvolvimento e produção.
2. **Como engenheiro de dados**, quero definir e implementar as tabelas e relacionamentos iniciais em PostgreSQL, para que o banco de dados armazene dados estruturados.

---

## Tarefas e Atividades

### 1.1 Configuração do Ambiente com Docker
- **Atividade:** Instalar Docker no ambiente local (se necessário) e criar contêineres para PostgreSQL e demais serviços essenciais.
- **Critérios de Aceitação:** Docker instalado, contêineres criados com Docker Compose, rodando de forma consistente no ambiente de desenvolvimento.
- **Status de Pronto:** Ambiente local executando PostgreSQL em um contêiner Docker.

### 1.2 Configuração do PostgreSQL com Tabelas Básicas
- **Atividade:** Estruturar e implementar tabelas iniciais para o armazenamento de dados de teste, incluindo valores, resultados e limites, usando SQL.
- **Critérios de Aceitação:** Tabelas básicas criadas com os tipos de dados definidos; relacionamentos principais implementados e funcionando.
- **Status de Pronto:** Banco de dados PostgreSQL populado com a estrutura inicial de tabelas e com dados de teste.

### 1.3 Documentação do Ambiente e Configuração do Banco
- **Atividade:** Documentar os passos para instalação, configuração do Docker e criação das tabelas iniciais no banco de dados.
- **Critérios de Aceitação:** Documentação clara e detalhada, com instruções para reprodução do ambiente e detalhes das tabelas.
- **Status de Pronto:** Documentação completa e acessível a todos os desenvolvedores para assegurar a reprodutibilidade.

---

## Definição de Pronto
Para a Sprint 1 ser considerada completa:
- O ambiente de desenvolvimento deve estar configurado com Docker, rodando PostgreSQL em um contêiner.
- As tabelas iniciais e relacionamentos do banco de dados devem estar criados e testados.
- Documentação do ambiente e banco de dados disponível para a equipe.

Essa estrutura para a Sprint 1 permitirá uma base sólida para o desenvolvimento do sistema, facilitando o trabalho nas sprints seguintes.

---

## 1.1 Passos para Configuração do Ambiente com Docker

### Instalação do Docker
1. **Baixe e Instale o Docker:**
   - Acesse Docker Desktop e baixe a versão para seu sistema operacional.
   - Siga as instruções de instalação para configurar o Docker em sua máquina.

2. **Verifique a Instalação:**
   - Abra um terminal (Prompt de Comando ou PowerShell no Windows).
   - Execute o comando:
     ```bash
     docker --version
     ```
   - Isso deve exibir a versão do Docker instalada.

### Criação do Arquivo `docker-compose.yml`
1. **Crie um diretório para o projeto:**
   ```bash
   mkdir data-plat
   cd data-plat
   ```
   
2. Criação do Arquivo `docker-compose.yml`

  - Abra um editor de texto e adicione o seguinte conteúdo:

```yaml
services:
  db:
    image: postgres:latest
    environment:
      POSTGRES_USER: cafrunikuhn
      POSTGRES_PASSWORD: admin
      POSTGRES_DB: data_plat
    ports:
      - "5432:5432"
    volumes:
      - pgdata:/var/lib/postgresql/data

volumes:
  pgdata:
```

## 1.2 Configuração do PostgreSQL com Tabelas Básicas
   
### Iniciar o Contêiner

1. **Inicie o contêiner com Docker Compose:**

-	No terminal, dentro do diretório do projeto, execute:
 ``` 
docker-compose up -d
```
-	O parâmetro -d inicia o contêiner em modo destacado (em segundo plano).

2.	**Verifique se o contêiner está em execução:**
-	Use o comando:
```
docker ps
```
-	Você deve ver o contêiner listado como data-plat-db-1.

### Acessar o Banco de Dados

1.	**Acesse o contêiner PostgreSQL:**
o	Execute o seguinte comando para abrir o cliente psql:
```
docker exec -it data-plat-db-1 psql -U cafrunikuhn -d data_plat
```
### Verificar Persistência dos Dados

1.	**Crie uma tabela e insira dados:**
```
CREATE TABLE test_table (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100)
);

INSERT INTO test_table (name) VALUES ('Test Data 1'), ('Test Data 2');
```

2.	**Verifique os dados inseridos:**
```
SELECT * FROM test_table;
```
4.	**Pare o contêiner:**
```
docker-compose down
```
6.	**Reinicie o contêiner:**
```
docker-compose up -d
```
8.	**Acesse novamente o contêiner:**
```
docker exec -it data-plat-db-1 psql -U cafrunikuhn -d data_plat
```
10.	**Verifique se os dados ainda estão presentes:**
```
SELECT * FROM test_table;
```
### Debug do Contêiner (Opcional)
Se você precisar depurar o contêiner, use o seguinte comando:
```
docker debug data-plat-db-1
```

### Conclusão
Este guia fornece um passo a passo completo para configurar o ambiente Docker com PostgreSQL, incluindo a verificação da persistência dos dados e como acessar o banco de dados.

Documentação e Passo a Passo: Configuração e Manipulação de Tabelas no PostgreSQL com Docker
Este documento fornece instruções detalhadas para:
1.	Listar tabelas no PostgreSQL dentro de um contêiner Docker.
2.	Excluir tabelas específicas.
3.	Comandos SQL para manipulação de tabelas.
4.	
Pré-requisitos
•	Ter o Docker e o PostgreSQL configurados e em execução.
•	Acesso ao contêiner Docker com o PostgreSQL.
________________________________________
1. Listando Tabelas no Banco de Dados PostgreSQL
Para listar as tabelas de um banco de dados específico dentro do contêiner Docker, siga os passos abaixo:
Passo 1: Acessar o Banco de Dados PostgreSQL
Execute o comando abaixo no terminal para entrar no contêiner e acessar o banco de dados data_plat:

```
docker exec -it data-plat-db-1 psql -U cafrunikuhn -d data_plat
```

•	docker exec -it: Executa um comando interativo no contêiner.
•	data-plat-db-1: Nome do contêiner Docker.
•	psql -U cafrunikuhn -d data_plat: Comando para abrir o prompt psql do PostgreSQL com o usuário e banco de dados especificados.
Passo 2: Listar as Tabelas Existentes
No prompt do PostgreSQL, execute o comando para listar todas as tabelas:

```
\dt
```

Esse comando exibe uma lista de todas as tabelas no banco de dados data_plat.
Passo 3: Sair do Prompt do PostgreSQL
Para sair do prompt, basta digitar:

```
\q
```
________________________________________
2. Excluindo Tabelas no PostgreSQL
Para remover uma tabela específica do banco de dados PostgreSQL, siga as instruções abaixo.
Passo 1: Acessar o Banco de Dados PostgreSQL
No terminal, acesse o contêiner e o banco de dados da mesma forma:
docker exec -it data-plat-db-1 psql -U cafrunikuhn -d data_plat
Passo 2: Executar o Comando para Excluir a Tabela
No prompt do PostgreSQL, execute o comando DROP TABLE para excluir a tabela desejada. Substitua nome_da_tabela pelo nome da tabela que você deseja excluir.

```
DROP TABLE nome_da_tabela;
```

Observação
Se quiser excluir a tabela apenas se ela existir, evitando erros caso a tabela não esteja presente, use o seguinte comando:
DROP TABLE IF EXISTS nome_da_tabela;
Este comando exclui a tabela e todos os dados nela de forma permanente.
Passo 3: Sair do Prompt do PostgreSQL
Para finalizar, digite o comando para sair do prompt:

```
\q
```
________________________________________
Resumo dos Comandos Utilizados

| Comando                                    | Função                                         |
|--------------------------------------------|------------------------------------------------|
| `docker exec -it <container> psql -U <user> -d <db>` | Acessa o banco de dados PostgreSQL no contêiner Docker |
| `\dt`                                      | Lista todas as tabelas do banco de dados       |
| `DROP TABLE nome_da_tabela;`               | Exclui uma tabela específica                   |
| `DROP TABLE IF EXISTS nome_da_tabela;`     | Exclui uma tabela apenas se ela existir        |
| `\q`                                       | Sai do prompt do PostgreSQL                    |


Este guia deve ajudá-lo a gerenciar as tabelas em um banco de dados PostgreSQL em contêineres Docker de maneira segura e eficiente.

Resumo dos Comandos Utilizados
Comando	Função
docker exec -it <container> psql -U <user> -d <db>	Acessa o banco de dados PostgreSQL no contêiner Docker
\dt	Lista todas as tabelas do banco de dados
DROP TABLE nome_da_tabela;	Exclui uma tabela específica
DROP TABLE IF EXISTS nome_da_tabela;	Exclui uma tabela apenas se ela existir
\q	Sai do prompt do PostgreSQL
Este guia deve ajudá-lo a gerenciar as tabelas em um banco de dados PostgreSQL em contêineres Docker de maneira segura e eficiente.

## Gerando banco de dados através de arquivo SQL:

1. Crie um arquivo chamado `sprint1_test_table.sql` em seu diretório de projeto com o seguinte conteúdo:

```
CREATE TABLE dut_completo (
    id SERIAL PRIMARY KEY,
    lot VARCHAR(50),
    version VARCHAR(50),
    date DATE
);

CREATE TABLE teste (
    id SERIAL PRIMARY KEY,
    dut_id INT NOT NULL,
    test_name VARCHAR(255) NOT NULL,  -- Ex.: "Continuidade", "Leakage"
    pin INT,
    temperature DECIMAL(5,2),
    voltage DECIMAL(5,2),
    result VARCHAR(255),  
    test_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    FOREIGN KEY (dut_id) REFERENCES dut_completo(id) ON DELETE CASCADE
);
```

2. Executar o Arquivo SQL no PostgreSQL:

Para executar o arquivo SQL e criar os bancos de dados e as tabelas, siga os passos abaixo:

Passo 1: Acesse o Contêiner PostgreSQL
No terminal, acesse o contêiner do PostgreSQL:

```
docker exec -it data-plat-db-1 psql -U your_user
```

Passo 2: Execute o Arquivo SQL
Com o prompt do PostgreSQL aberto, execute o arquivo SQL com o seguinte comando:

```
\i /path/to/your/sprint1_test_table.sql
```

Substitua /path/to/your/setup.sql pelo caminho real onde você salvou o arquivo sprint1_test_table.sql dentro do contêiner. Você pode precisar copiar o arquivo para o contêiner ou montá-lo como um volume no Docker.

3. Verificar a Criação das Tabelas:

Após executar o arquivo SQL, você pode verificar se as tabelas foram criadas corretamente usando o comando:

```
\dt
```

Isso exibirá uma lista de todas as tabelas no banco de dados data_plat.


