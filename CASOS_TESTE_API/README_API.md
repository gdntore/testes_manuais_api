# 🌐 Casos de Teste — API REST

Casos de teste para validação da API REST pública [ServeRest](https://serverest.dev/), cobrindo operações CRUD com foco na validação de status codes HTTP, estrutura das respostas JSON e regras de negócio.

---

## 📋 Informações do Projecto

| Campo | Detalhe |
|---|---|
| Testador | Mateus Toré |
| Versão | V_1 |
| Sistema | https://serverest.dev/ |
| Ambiente | Postman |
| Total de Casos | 9 |

---

## 📊 Resumo de Execução

| Status | Quantidade |
|---|---|
| ✅ Aprovado | 5 |
| ⏳ Não executado | 4 |
| ❌ Reprovado | 0 |

---

## 🔄 Cobertura por Método HTTP

| Método | Casos | Descrição |
|---|---|---|
| GET | 2 | Busca de recursos |
| POST | 2 | Criação de recursos |
| DELETE | 1 | Remoção de recursos |
| PUT | — | Em desenvolvimento |

---

## 🧪 Casos de Teste

| ID | Título | Método | Endpoint | Prioridade | Status |
|---|---|---|---|---|---|
| CT_API_1 | Buscar todos os utilizadores cadastrados | GET | /usuarios | Alta | ✅ Aprovado |
| CT_API_2 | Cadastrar utilizador sem dados obrigatórios | POST | /usuarios | Alta | ✅ Aprovado |
| CT_API_3 | Cadastrar utilizador com dados correctos | POST | /usuarios | Alta | ✅ Aprovado |
| CT_API_4 | Buscar utilizador por ID | GET | /usuarios/:id | Alta | ✅ Aprovado |
| CT_API_5 | Excluir utilizador | DELETE | /usuarios/:id | Alta | ✅ Aprovado |
| CT_API_6 | — | — | — | — | ⏳ Pendente |
| CT_API_7 | — | — | — | — | ⏳ Pendente |
| CT_API_8 | — | — | — | — | ⏳ Pendente |
| CT_API_9 | — | — | — | — | ⏳ Pendente |

---

## 📁 Ficheiros

| Ficheiro | Descrição |
|---|---|
| `CT_API.json` | Casos de teste completos em formato JSON |
| `CT_API.xlsx` | Casos de teste em formato Excel |
| `SERVEREST_API_TESTE.postman_collection` | Postman_Collection |

---

## 🔍 O que foi validado

- Status codes HTTP correctos (200, 201, 400, 404)
- Estrutura e formato das respostas em JSON
- Validação de campos obrigatórios no body da requisição
- Busca de recursos por ID
- Remoção de recursos e validação da resposta

---

## 📐 Estrutura dos Casos de Teste

Cada caso de teste segue a estrutura:

```
- ID
- Título
- Método HTTP
- Endpoint
- Prioridade
- Pré-Condições
- Dados de Entrada (body JSON)
- Nº de Passos
- Passos (BDD & Gherkin)
- Resultado Esperado
- Critério de Aceite
- Status
```
