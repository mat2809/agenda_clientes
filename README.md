📘 Gerenciador de Clientes — Documentação Oficial
Bem-vindo ao Gerenciador de Clientes, uma aplicação desenvolvida em Python com interface gráfica, voltada para iniciantes que desejam aprender na prática conceitos de programação, banco de dados e interfaces gráficas.

Este projeto permite o gerenciamento de informações básicas de clientes — como nome, sobrenome, email e CPF — utilizando SQLite como sistema de banco de dados e Tkinter para a interface gráfica.

🎯 Objetivo do Projeto
O objetivo deste sistema é servir como um exemplo didático para estudantes iniciantes em Python, SQL/SQLite e desenvolvimento de interfaces com Tkinter. Com ele, é possível aprender como:

Criar uma interface gráfica funcional.

Conectar um sistema a um banco de dados.

Realizar operações básicas de CRUD (Create, Read, Update, Delete).

🛠️ Funcionalidades
A aplicação permite:

✅ Adicionar novos clientes ao banco de dados.

✅ Visualizar todos os clientes em uma tabela interativa.

✅ Buscar clientes por nome, sobrenome, email ou CPF.

✅ Atualizar os dados de clientes existentes.

✅ Excluir clientes cadastrados.

Todos os dados são armazenados localmente em um arquivo SQLite (clientes.db).

🗂️ Estrutura do Projeto
O projeto é modularizado em três arquivos principais:

Gui.py
Responsável pela criação da interface gráfica usando Tkinter.

Contém os campos de entrada, botões de ação e uma tabela Treeview para exibir os clientes.

Conecta-se à classe Backend para realizar as operações no banco de dados.

Backend.py
Contém a lógica de acesso ao banco de dados SQLite.

Realiza todas as operações de banco (inserção, consulta, atualização e exclusão).

Usa consultas parametrizadas para maior segurança.

application.py
Arquivo principal que inicializa a aplicação.

Executa a criação da base de dados (se necessário) e exibe a janela da interface gráfica.

✅ Pré-Requisitos
Para executar o projeto, você precisará de:

Python 3.8 ou superior

Download do Python

Tkinter

Como Usar a Aplicação
Interface:
Campos de Entrada: Nome, Sobrenome, Email e CPF

Botões:

Adicionar: Cadastra um novo cliente

Atualizar: Altera os dados do cliente selecionado

Excluir: Remove o cliente selecionado

Buscar: Filtra os clientes com base nos dados inseridos

Limpar: Limpa os campos de entrada

Tabela (Treeview): Exibe os clientes cadastrados

Exemplo de Uso:
➕ Adicionar um cliente:
Preencha todos os campos

Clique em “Adicionar”

🔍 Buscar cliente:
Insira nome, email, ou CPF

Clique em “Buscar”

✏️ Atualizar cliente:
Selecione um cliente na tabela

Altere os dados

Clique em “Atualizar”

❌ Excluir cliente:
Selecione um cliente

Clique em “Excluir”

🧱 Estrutura do Banco de Dados (clientes.db)
A tabela clientes possui a seguinte estrutura:

Campo	Tipo	Descrição
id	INTEGER	Chave primária (auto incremento)
nome	TEXT	Nome do cliente
sobrenome	TEXT	Sobrenome do cliente
email	TEXT	Email do cliente
cpf	TEXT	CPF do cliente

Essa tabela é criada automaticamente na primeira execução.

📦 Criando um Executável com PyInstaller
Você pode converter o projeto para um arquivo executável com os seguintes comandos:

1. Instale o PyInstaller
bash
Copiar
Editar
pip install pyinstaller
2. Gere o executável
bash
Copiar
Editar
pyinstaller --onefile --noconsole application.py
O executável será gerado na pasta dist/ como application.exe.

🧪 Dicas de Solução de Problemas
Erro	Solução
ModuleNotFoundError: No module named 'tkinter'	Verifique se Tkinter está instalado. No Linux: sudo apt install python3-tk
Nada acontece ao executar o .exe	Tente rodar o executável pelo terminal para visualizar erros ocultos
A tabela não atualiza	Verifique se o arquivo clientes.db está na mesma pasta da aplicação

🎓 O que você aprende com este projeto
Python: Classes, métodos estáticos, organização de código em módulos

SQLite: Criação e manipulação de banco de dados local com SQL

Tkinter: Criação de GUIs com campos de entrada, botões e tabelas

Boas práticas: Separação entre lógica e interface, uso de queries seguras

Distribuição: Criação de executáveis com PyInstaller

🚀 Próximos Passos (Sugestões de melhoria)
✅ Validação do formato de CPF e email

✅ Exportar dados para CSV ou Excel

✅ Filtro por múltiplos campos combinados

✅ Melhorias visuais com cores e ícones

✅ Adição de paginação ou busca por ID

📅 Última Atualização
27 de junho de 2025