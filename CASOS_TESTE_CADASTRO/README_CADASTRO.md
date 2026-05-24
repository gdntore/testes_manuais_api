# 📝 Casos de Teste — Cadastro de Utilizadores

Casos de teste manuais para validação do fluxo de cadastro da aplicação [ServeRest](https://front.serverest.dev/cadastrarusuarios), cobrindo validações de campos obrigatórios, formatos e regras de negócio.

---

## 📋 Informações do Projecto

| Campo | Detalhe |
|---|---|
| Testador | Mateus Toré |
| Versão | V_1 |
| Sistema | https://front.serverest.dev/cadastrarusuarios |
| Ambiente | Google Chrome \| Brave \| Firefox |
| Total de Casos | 9 |

---

## 📊 Resumo de Execução

| Status | Quantidade |
|---|---|
| ✅ Aprovado | 6 |
| ⏳ Não executado | 3 |
| ❌ Reprovado | 0 |

---

## 🧪 Casos de Teste

| ID | Título | Prioridade | Status |
|---|---|---|---|
| CT_CADASTRO_1 | Cadastrar com todos os campos vazios | Alta | ✅ Aprovado |
| CT_CADASTRO_2 | Cadastrar com o campo nome vazio | Alta | ✅ Aprovado |
| CT_CADASTRO_3 | Cadastrar com o campo senha vazio | Alta | ✅ Aprovado |
| CT_CADASTRO_4 | Cadastrar com o campo e-mail vazio | Alta | ✅ Aprovado |
| CT_CADASTRO_5 | Cadastrar com o formato do e-mail errado | Alta | ✅ Aprovado |
| CT_CADASTRO_6 | Cadastro já existente | Alta | ✅ Aprovado |
| CT_CADASTRO_7 | — | — | ⏳ Pendente |
| CT_CADASTRO_8 | — | — | ⏳ Pendente |
| CT_CADASTRO_9 | — | — | ⏳ Pendente |

---

## 📁 Ficheiros

| Ficheiro | Descrição |
|---|---|
| `CT_CADASTRO.json` | Casos de teste completos em formato JSON |
| `CT_CADASTRO.xlsx` | Casos de teste em formato Excel |

---

## 🔍 O que foi testado

- Submissão do formulário com todos os campos vazios
- Validação individual de cada campo obrigatório (Nome, E-mail, Senha)
- Validação do formato do e-mail
- Comportamento ao tentar cadastrar um utilizador já existente

---

## 📐 Estrutura dos Casos de Teste

Cada caso de teste segue a estrutura:

```
- ID
- Título
- Cenário do Teste
- Prioridade
- Pré-Condições
- Dados de Entrada
- Nº de Passos
- Passos (BDD & Gherkin)
- Resultado Esperado
- Critério de Aceite
- Status
```
