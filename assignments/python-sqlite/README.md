# 📘 Assignment: Persistência de Dados com SQLite

## 🎯 Objective

Crie um gerenciador de lista de leitura em Python usando o módulo `sqlite3`, que já faz parte da biblioteca padrão. Você praticará como criar um banco de dados, salvar registros de forma persistente e executar operações CRUD.

## 📝 Tasks

### 🛠️ Criar o Banco de Dados e a Tabela

#### Descrição
Configure o arquivo `reading_list.db` e crie uma tabela para armazenar livros. O programa deve poder ser executado novamente sem falhar se o banco de dados e a tabela já existirem.

#### Requisitos
O programa concluído deve:

- Importar e usar o módulo `sqlite3`, sem instalar bibliotecas externas.
- Criar a tabela `books` com `id` como chave primária e os campos `title` e `author` como texto obrigatório.
- Consultar e exibir os livros armazenados.

### 🛠️ Adicionar e Listar Livros

#### Descrição
Permita que o usuário adicione livros à lista e consulte todos os registros salvos.

#### Requisitos
O programa concluído deve:

- Solicitar o título e o autor de um livro e inserir esses valores na tabela.
- Usar parâmetros nas consultas SQL em vez de concatenar valores fornecidos pelo usuário ao comando SQL.
- Exibir os livros com seus identificadores, títulos e autores.
- Manter os registros disponíveis depois que o programa for encerrado e executado novamente.

### 🛠️ Atualizar e Remover Livros

#### Descrição
Complete o gerenciador permitindo editar ou remover um livro usando seu identificador.

#### Requisitos
O programa concluído deve:

- Atualizar o título e o autor de um livro selecionado pelo `id`.
- Remover um livro selecionado pelo `id`.
- Informar ao usuário quando o identificador informado não corresponder a nenhum livro.
- Usar parâmetros nas consultas SQL para todas as operações que recebem valores do usuário.