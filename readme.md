# API de Gerenciamento de Pedidos 📦

Um projeto de API RESTful para gerenciamento de pedidos, construído com FastAPI, SQLAlchemy e uma arquitetura limpa (camadas de Controller e Service).

---

## 🚀 Sobre o Projeto

Este projeto implementa um sistema básico de gerenciamento de pedidos, permitindo operações de CRUD (Criar, Ler, Atualizar, Deletar) para pedidos. O objetivo é demonstrar o uso de FastAPI com uma arquitetura desacoplada, separando a lógica de negócios (Services) da lógica de HTTP (Controllers).

### ✨ Principais Funcionalidades

* **CRUD completo** para Pedidos.
* **Geração automática de documentação** interativa com Swagger UI e ReDoc.
* **Validação de dados** de entrada e saída usando Pydantic.
* **Arquitetura em camadas** (Controllers, Services) para fácil manutenção e teste.
* **Comunicação com banco de dados** relacional (PostgreSQL/SQLite) via SQLAlchemy ORM.

---

## 💻 Tecnologias Utilizadas

* **Python 3.10+**
* **FastAPI:** O framework web principal.
* **Uvicorn:** O servidor ASGI para rodar o FastAPI.
* **SQLAlchemy:** O ORM para interagir com o banco de dados.
* **Pydantic:** Para validação e serialização de dados (Schemas).

---

## 🔧 Instalação e Execução

Siga os passos abaixo para configurar e executar o projeto em sua máquina local.

### 1. Pré-requisitos

* Python 3.10 ou superior
* Git (para clonar o repositório)

### 2. Clone o Repositório

git clone [https://github.com/SanNes-hub/Portif-lio.git](https://github.com/SanNes-hub/Portif-lio.git)
cd Portif-lio
```

### 3. Crie e Ative um Ambiente Virtual (Venv)

É uma boa prática isolar as dependências do projeto.

# Criar o ambiente virtual
python -m venv venv

# Ativar no Windows
.\venv\Scripts\activate

# Ativar no macOS/Linux
source venv/bin/activate

### 4. Instale as Dependências

Este projeto usa um arquivo `requirements.txt` para gerenciar as dependências.

pip install -r requirements.txt

*(**Nota:** Se você ainda não criou o `requirements.txt`, rode `pip freeze > requirements.txt` no seu terminal para criá-lo com as bibliotecas que você já instalou.)*

### 5. Configure o Banco de Dados

*(Esta seção é um exemplo. Adapte para seu projeto.)*

O projeto espera um arquivo `.env` para carregar a URL de conexão do banco de dados.

1.  Crie um arquivo chamado `.env` na raiz do projeto.
2.  Adicione sua string de conexão:

    ```env
    DATABASE_URL="postgresql://USUARIO:SENHA@localhost:5432/NOME_DO_BANCO"
    ```

### 6. Execute o Servidor

Com o ambiente virtual ativado e as dependências instaladas, inicie o servidor Uvicorn.

uvicorn main:app --reload


* `main` é o nome do seu arquivo Python principal (ex: `main.py`).
* `app` é o nome da sua instância do FastAPI (ex: `app = FastAPI()`).
* `--reload` faz o servidor reiniciar automaticamente após qualquer alteração no código.

---

## 📚 Como Usar (Endpoints da API)

Após iniciar o servidor, a documentação interativa da API estará disponível automaticamente. Você pode usá-la para testar todos os endpoints.

* **Swagger UI:** [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
* **ReDoc:** [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)

Prints dos testes realizados




