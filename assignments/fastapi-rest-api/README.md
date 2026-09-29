# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Construa uma API REST com FastAPI para gerenciar tarefas e pratique rotas HTTP, validação de dados, códigos de status e documentação automática. Os dados podem ficar em memória, sem banco de dados.

## 📝 Tasks

### 🛠️ Create the FastAPI App and Read Endpoints

#### Descrição
Crie e execute uma aplicação FastAPI para gerenciar tarefas. Cada tarefa deve ter um identificador inteiro, um título e um estado de conclusão.

#### Requisitos
A aplicação deve:

- Iniciar localmente com FastAPI.
- Disponibilizar `GET /health`, retornando `{ "status": "ok" }`.
- Disponibilizar `GET /tasks`, retornando a lista de tarefas armazenadas em memória.
- Representar cada tarefa com os campos `id`, `title` e `completed`.

### 🛠️ Create and Retrieve Tasks

#### Descrição
Implemente a criação de tarefas e a consulta de uma tarefa específica pelo identificador, validando os dados recebidos no corpo da requisição.

#### Requisitos
A aplicação deve:

- Disponibilizar `POST /tasks` para criar uma tarefa com título obrigatório e estado `completed` inicialmente falso.
- Validar o corpo da requisição usando um modelo do Pydantic.
- Retornar a tarefa criada com código HTTP `201 Created`.
- Disponibilizar `GET /tasks/{task_id}` e retornar `404 Not Found` quando o identificador não existir.

### 🛠️ Update and Delete Tasks

#### Descrição
Complete as operações da API permitindo atualizar e excluir tarefas existentes.

#### Requisitos
A aplicação deve:

- Disponibilizar `PUT /tasks/{task_id}` para atualizar uma tarefa existente.
- Disponibilizar `DELETE /tasks/{task_id}` para excluir uma tarefa existente.
- Retornar `404 Not Found` para operações feitas com identificadores inexistentes.
- Usar códigos HTTP adequados para as operações de atualização e exclusão.
- Permitir testar as rotas pela documentação interativa em `/docs`.
