# 🔐 Casos de Teste — Login

Casos de teste manuais para validação do fluxo de login da aplicação [ServeRest](https://front.serverest.dev/login), cobrindo cenários positivos e negativos com foco em regras de negócio e experiência do utilizador.

---

## 📋 Informações do Projecto

| Campo | Detalhe |
|---|---|
| Testador | Mateus Toré |
| Versão | V_1 |
| Sistema | https://front.serverest.dev/login |
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
| CT_LOGIN_1 | Campos Vazios | Alta | ✅ Aprovado |
| CT_LOGIN_2 | E-mail Válido e Senha Inválida | Alta | ✅ Aprovado |
| CT_LOGIN_3 | E-mail Inválido e Senha Válida | Alta | ✅ Aprovado |
| CT_LOGIN_4 | Ambos Válidos | Alta | ✅ Aprovado |
| CT_LOGIN_5 | O botão "Entrar" Visível | Alta | ✅ Aprovado |
| CT_LOGIN_6 | Cadastre-se | Alta | ✅ Aprovado |
| CT_LOGIN_7 | — | — | ⏳ Pendente |
| CT_LOGIN_8 | — | — | ⏳ Pendente |
| CT_LOGIN_9 | — | — | ⏳ Pendente |

---

## 📁 Ficheiros

| Ficheiro | Descrição |
|---|---|
| `CT_LOGIN.json` | Casos de teste completos em formato JSON |
| `CT_LOGIN.xlsx` | Casos de teste em formato Excel |

---

## 🔍 O que foi testado

- Validação de campos obrigatórios (email e senha vazios)
- Comportamento com email válido e senha incorrecta
- Comportamento com formato de email inválido (sem `@`)
- Fluxo de login com credenciais correctas
- Visibilidade e funcionamento do botão de acção
- Redirecionamento para página de cadastro

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
