# masterclass-sentry

Exemplo de API base para configurar o Sentry.

## Chamadas de API

```sh
# Cria Usuário 
curl -d '{
    "name": "",
    "email": "rubens@gmail.com",
    "password": "123",
    "role": "teste"
}' -H "Content-Type: application/json" -X POST http://localhost:3000/users


# Autentica Usuário
curl -d '{
    "email": "rubens@gmail.com",
    "password": "123"
}' -H "Content-Type: application/json" -X POST http://localhost:3000/users/auth


# Lista Usuários
curl -H "Content-Type: application/json" -H "Authorization: Bearer $TOKEN" -X GET http://localhost:3000/users 
```
