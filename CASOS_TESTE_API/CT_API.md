# 🧪 Casos de Teste – API (ServeRest)

**Projeto:** Portfólio QA  
**Tipo de Teste:** Testes de API REST  
**Ferramenta:** Postman  
**API Pública:** https://serverest.dev  

---

## 📌 CT_API_1 – Buscar todos os usuários cadastrados

| Campo | Descrição |
|------|----------|
| **Método** | GET |
| **Endpoint** | `/usuarios` |
| **Prioridade** | Alta |
| **Pré-condições** | API disponível; Existirem usuários cadastrados |
| **Dados de Entrada** | N/A |

### 🧾 Passos (BDD)
- **Dado** que a API esteja disponível  
- **Quando** enviar a request GET  
- **E** clicar em "Send"  

### ✅ Resultado Esperado
- Status Code 200  
- Response em formato JSON  
- Retornar informações dos usuários cadastrados  

### 📊 Resultado Obtido
- Status Code 200  
- Response em formato JSON  
- Dados dos usuários retornados  

**Status:** ✅ Aprovado

---

## 📌 CT_API_2 – Cadastrar usuário sem dados obrigatórios

| Campo | Descrição |
|------|----------|
| **Método** | POST |
| **Endpoint** | `/usuarios` |
| **Prioridade** | Alta |
| **Pré-condições** | API disponível |
| **Dados de Entrada** | N/A |

### 🧾 Passos (BDD)
- **Dado** que a API esteja disponível  
- **Quando** enviar a request POST sem body  
- **E** clicar em "Send"  

### ✅ Resultado Esperado
- Status Code 400  
- Response em formato JSON  
- Retornar mensagens de erro para campos obrigatórios  

### 📊 Resultado Obtido
- Status Code 400  
- Mensagens de erro retornadas conforme esperado  

**Status:** ✅ Aprovado

---

## 📌 CT_API_3 – Cadastrar usuário com dados válidos

| Campo | Descrição |
|------|----------|
| **Método** | POST |
| **Endpoint** | `/usuarios` |
| **Prioridade** | Alta |
| **Pré-condições** | API disponível; Usuário não cadastrado |
| **Dados de Entrada** | Nome, email, senha e perfil válidos |

### 🧾 Passos (BDD)
- **Dado** que a API esteja disponível  
- **Quando** enviar a request POST com dados válidos  
- **E** clicar em "Send"  

### ✅ Resultado Esperado
- Status Code 201  
- Usuário cadastrado com sucesso  
- Retornar ID do usuário criado  

### 📊 Resultado Obtido
- Status Code 201  
- Mensagem de cadastro realizado com sucesso  
- ID do usuário retornado  

**Status:** ✅ Aprovado

---

## 📌 CT_API_4 – Buscar usuário por ID

| Campo | Descrição |
|------|----------|
| **Método** | GET |
| **Endpoint** | `/usuarios/{id}` |
| **Prioridade** | Alta |
| **Pré-condições** | API disponível; Usuário cadastrado |
| **Dados de Entrada** | ID válido do usuário |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja cadastrado  
- **Quando** enviar uma request GET informando o ID  
- **E** clicar em "Send"  

### ✅ Resultado Esperado
- Status Code 200  
- Retornar dados do usuário correspondente ao ID  
- Response em formato JSON  

### 📊 Resultado Obtido
- Status Code 200  
- Dados do usuário retornados conforme esperado  

**Status:** ✅ Aprovado

---

## 📌 CT_API_5 – Excluir usuário

| Campo | Descrição |
|------|----------|
| **Método** | DELETE |
| **Endpoint** | `/usuarios/{id}` |
| **Prioridade** | Alta |
| **Pré-condições** | API disponível; Usuário cadastrado |
| **Dados de Entrada** | ID válido do usuário |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja cadastrado  
- **Quando** enviar uma request DELETE informando o ID  
- **E** clicar em "Send"  

### ✅ Resultado Esperado
- Status Code 200  
- Mensagem de exclusão realizada com sucesso  

### 📊 Resultado Obtido
- Status Code 200  
- Mensagem de exclusão retornada conforme esperado  

**Status:** ✅ Aprovado

---

## 🧠 Observações
- Testes executados manualmente via Postman  
- API utilizada apenas para fins educacionais  
- Dados não persistem permanentemente  
