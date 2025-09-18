# 📘 Projeto Matrícula CRUD

Aplicação desenvolvida em **Python/Django** para gerenciamento de alunos e matrículas, implementando operações de **CRUD (Create, Read, Update, Delete)**.

---

## 🔧 Requisitos

- Python 3.7+  
- pip (gerenciador de pacotes do Python)  
- Virtualenv (opcional, mas recomendado)  
- SQLite (já incluso no projeto)  

---

## 📥 Instalação e Execução

Copie e cole o bloco abaixo no terminal:

```bash
# --- COPIAR & COLAR: passos de instalação e execução ---
# 1) Clonar repositório e entrar na pasta
git clone https://github.com/victormanoelrego/projeto_matricula_CRUD.git
cd projeto_matricula_CRUD || exit 1

# 2) Criar ambiente virtual (local: .venv)
python -m venv .venv

# 3) Ativar o ambiente virtual
# -> Linux / macOS:
# source .venv/bin/activate
# -> Windows PowerShell:
# .venv\Scripts\Activate.ps1
# -> Windows (cmd.exe):
# .venv\Scripts\activate.bat

# 4) Atualizar pip e instalar dependências
python -m pip install --upgrade pip setuptools wheel
pip install -r requirements.txt

# 5) Criar migrações e aplicar
python manage.py makemigrations
python manage.py migrate

# 6) (Opcional) Criar superuser para acessar o admin
python manage.py createsuperuser

# 7) Rodar servidor de desenvolvimento
python manage.py runserver 0.0.0.0:8000

# -> Acesse: http://127.0.0.1:8000/ ou http://localhost:8000/
# --- FIM ---


