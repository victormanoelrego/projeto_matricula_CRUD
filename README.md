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
# --- COPIAR & COLAR: passos de instalação e execução ---
# 1) Clonar repositório e entrar na pasta
git clone https://github.com/victormanoelrego/projeto_matricula_CRUD.git
cd projeto_matricula_CRUD || exit 1

# 2) Criar ambiente virtual (local: .venv)
python -m venv .venv

# 3) Ativar o ambiente virtual
# -> Linux / macOS (execute essa linha no terminal Unix):
# source .venv/bin/activate
# -> Windows PowerShell (execute esta linha no PowerShell):
# .venv\Scripts\Activate.ps1
# -> Windows (cmd.exe):
# .venv\Scripts\activate.bat

# (Se preferir não ativar, pode chamar diretamente o pip do venv nas linhas abaixo:
# Linux/macOS: .venv/bin/pip install -r requirements.txt
# Windows: .venv\Scripts\pip.exe install -r requirements.txt
# )

# 4) Atualizar pip e instalar dependências
python -m pip install --upgrade pip setuptools wheel
pip install -r requirements.txt

# 5) Criar migrações e aplicar (garante que o DB esteja pronto)
python manage.py makemigrations
python manage.py migrate

# 6) (Opcional) Criar um superuser para acessar o admin
# execute e siga as instruções interativas:
python manage.py createsuperuser

# 7) Rodar servidor de desenvolvimento
python manage.py runserver 0.0.0.0:8000

# -> Acesse: http://127.0.0.1:8000/ ou http://localhost:8000/
# --- FIM ---

