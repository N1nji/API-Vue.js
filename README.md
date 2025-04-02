# Teste de API - IntuitiveCare

## Descrição
Este projeto consiste em uma interface web desenvolvida com Vue.js que interage com um servidor em Python. 
O objetivo é buscar informações sobre operadoras de planos de saúde a partir de um arquivo CSV fornecido.

## Tecnologias Utilizadas
- **Python** (Flask para o servidor)
- **Vue.js** (Interface web)
- **PostgreSQL** (Banco de dados, se aplicável)
- **Postman** (Para testar a API)

## Configuração do Ambiente
### 1. Clonar o repositório
```sh
 git clone https://github.com/N1nji/API-Vue.js.git
 cd seu-repositorio
```

### 2. Configurar o ambiente Python
Certifique-se de ter o Python 3 instalado.

```sh
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Executar o Servidor
```sh
python app.py
```

O servidor rodará em `http://localhost:5000`.

## Endpoints da API
### **Buscar operadoras por texto**
`GET /buscar?query=<termo>`
- **Parâmetro:** `query` (string) - Texto a ser buscado
- **Resposta:** JSON com a lista de operadoras relevantes

Exemplo de chamada:
```sh
curl "http://localhost:5000/buscar?query=Unimed"
```

## Testando com Postman
Uma coleção do Postman foi criada para facilitar os testes.

### Importar a Coleção
1. Abra o Postman
2. Clique em **Import** e selecione o arquivo `postman_collection.json`
3. Execute as requisições disponíveis

## Executando a Interface Vue.js
### 1. Instalar Dependências
Certifique-se de ter o Node.js instalado.
```sh
cd frontend
npm install
```

### 2. Rodar o Projeto
```sh
npm run dev
```

A interface estará acessível em `http://localhost:5173` (ou outra porta especificada pelo Vite).



