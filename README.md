# Projeto Matrícula CRUD

Projeto simples de CRUD para gerenciamento de matrículas e alunos, feito com Python/Django.

---

## Requisitos

- Python 3.7+  
- pip  
- (Opcional) ambiente virtual (**venv** ou **virtualenv**)  
- SQLite (já incluso no projeto)  

---

## Instalação

1. Clone o repositório:

   ```bash
   git clone https://github.com/victormanoelrego/projeto_matricula_CRUD.git
   cd projeto_matricula_CRUD
(Opcional, mas recomendado) Crie e ative um ambiente virtual:

No Linux / MacOS:

bash
Copiar código
python3 -m venv venv
source venv/bin/activate
No Windows:

powershell
Copiar código
python -m venv venv
venv\Scripts\activate
Instale as dependências com o pip:

bash
Copiar código
pip install -r requirements.txt
Configuração do banco de dados
O projeto já possui um arquivo db.sqlite3, então não é necessário configurar outro banco por padrão.

Se quiser usar outro banco, ajuste as configurações no arquivo settings.py do Django:

DATABASES → ENGINE, NAME, USER, PASSWORD, etc.

Migrações
Execute as migrações para preparar o banco de dados:

bash
Copiar código
python manage.py makemigrations
python manage.py migrate
Execução
Para rodar o servidor de desenvolvimento:

bash
Copiar código
python manage.py runserver
Acesse no navegador:

cpp
Copiar código
http://127.0.0.1:8000/
