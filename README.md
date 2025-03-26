# API Doação de Livros 

Essa é uma API simples feita com Flask e SQLITE3 para fins de estudo da escola Vai Na Wb, ela permite cadstrar e listar livros doados

## Como rodar o projeto 

1. Faça o clone do repositorio: 
```bash 
git clone <URL_DO_REPOSITORIO>
cd nome-do-projeto
```

2. Crie um ambiente virtual (obrigatório):
```bash 
python -m venv venv
source venv/Scripts/activate 
```

3. Instale as dependências 
```bash
pip install -r requirements.txt
```

4. Inicie o servidor:
```bash 
python app.py 
```

> a API estará disponivel em: http://127.0.0.1:5000/

## Endpoints 

## POST /doar

Endpoint para cadastrar um novo livro 

**Formato de envio dos dados**
```json
{
    "titulo": "A Hipótese do Amor",
    "categoria": "Romance",
    "autor": "Ali Hazelwood",
    "image_url": "https://exemplo.com"
}
```

**Resposta 201 (Created)**
```json
{
    "mensagem": "Livro cadastrado com sucesso"
}
```
### GET /livros

Retorna todos os livros cadastrados em nossa API.

**Resposta (200)**:
```json
{
    "id":"1",
    "titulo": "A Hipótese do Amor",
    "categoria": "Romance",
    "autor": "Ali Hazelwood",
    "image_url": "https://exemplo.com"
}
```

---



