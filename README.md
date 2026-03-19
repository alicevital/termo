# 🎮 Termo API — Backend

Este projeto é uma API desenvolvida com **FastAPI** que implementa a lógica do jogo estilo *Termo*, onde o jogador tenta adivinhar uma palavra secreta em até 6 tentativas.

---

## 🧠 Sobre o jogo

O Termo é um jogo de palavras onde:

* O jogador precisa descobrir uma palavra secreta com 5 letras
* Ele tem **6 tentativas**
* A cada tentativa, recebe feedback:

| Cor        | Significado                      |
| ---------- | -------------------------------- |
| 🟩 Verde   | Letra correta na posição correta |
| 🟨 Amarelo | Letra correta na posição errada  |
| ⬜ Cinza    | Letra não existe na palavra      |

---

## ⚙️ Tecnologias utilizadas

* Python 3.12+
* FastAPI
* SQLAlchemy
* PostgreSQL
* Uvicorn

---

## 🚀 Como rodar o projeto

###  1. Clonar o repositório

```bash
git clone <url-do-repositorio>
cd termo
```

###  2. Criar e ativar ambiente virtual

```bash
python -m venv venv
```

### Windows:

```bash
venv\Scripts\activate
```

###  3. Instalar dependências

```bash
pip install -r requirements.txt
```

### 4. Criar banco de dados:

```sql
CREATE DATABASE termo;
```

###  5. Rodar a aplicação

```bash
uvicorn app.main:app --reload
```

###  6. Acessar documentação

Abra no navegador:

```
http://127.0.0.1:8000/docs
```

---

## 🎯 Estados do jogo

| Status  | Descrição                     |
| ------- | ----------------------------- |
| playing | Jogo em andamento             |
| win     | Jogador acertou a palavra     |
| lose    | Jogador esgotou as tentativas |

---

## ⚠️ Observações:

* A palavra secreta não é exposta na API
* O usuário está fixo (ID = 1) para simplificação
* O sistema ainda não valida se a palavra existe no dicionário

---

## 📌 Status do projeto

🚧 Em desenvolvimento

---

Se encontrar algum bug ou quiser melhorar o projeto, sinta-se à vontade para contribuir!
