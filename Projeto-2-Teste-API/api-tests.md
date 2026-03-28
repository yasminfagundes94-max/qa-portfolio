# 🔌 Testes de API

## 🔹 GET /users

**Objetivo:** Validar retorno de usuários

**Validações:**
- Status code 200
- Retorno com lista de usuários
- Campos obrigatórios presentes (id, name, email)

---

## 🔹 GET /users/1

**Objetivo:** Validar usuário específico

**Validações:**
- Status code 200
- ID corresponde ao solicitado
- Dados retornados corretamente

---

## 🔹 GET /users/999

**Objetivo:** Testar usuário inexistente

**Validações:**
- Retorno vazio ou erro
- Comportamento consistente da API

---

## 🔹 POST /users

**Objetivo:** Criar novo usuário

**Body:**
{
  "name": "Teste",
  "email": "teste@email.com"
}

**Validações:**
- Status code 201
- Retorno com dados enviados
- ID gerado
