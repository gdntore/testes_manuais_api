# 🧪 Casos de Teste – Cadastro de Usuários (ServeRest)

**Projeto:** Portfólio QA  
**Tipo de Teste:** Testes Funcionais / Testes Manuais  
**Sistema:** https://front.serverest.dev/cadastrarusuarios  
**API de Apoio:** https://serverest.dev  
**Navegadores:** Google Chrome | Brave | Firefox  

---

## 📌 CT_CADASTRO_1 – Cadastrar com todos os campos vazios

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Estar na página de cadastro |
| **Dados de Entrada** | N/A |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja na página de cadastro  
- **Quando** deixar os campos Nome, E-mail e Senha vazios  
- **E** clicar em "Cadastrar"  

### ✅ Resultado Esperado
- Cadastro não deve ser efetuado  
- Exibir mensagem informando que os campos são obrigatórios  

### 📊 Resultado Obtido
- Cadastro não efetuado  
- Mensagem de campos obrigatórios exibida  

**Status:** ✅ Aprovado

---

## 📌 CT_CADASTRO_2 – Cadastrar com campo Nome vazio

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Estar na página de cadastro |
| **Dados de Entrada** | E-mail válido e senha válida |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja na página de cadastro  
- **Quando** deixar o campo Nome vazio  
- **E** clicar em "Cadastrar"  

### ✅ Resultado Esperado
- Cadastro não deve ser efetuado  
- Exibir mensagem informando que o campo Nome é obrigatório  

### 📊 Resultado Obtido
- Cadastro não efetuado  
- Mensagem de campo Nome obrigatório exibida  

**Status:** ✅ Aprovado

---

## 📌 CT_CADASTRO_3 – Cadastrar com campo Senha vazio

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Estar na página de cadastro |
| **Dados de Entrada** | Nome válido e e-mail válido |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja na página de cadastro  
- **Quando** deixar o campo Senha vazio  
- **E** clicar em "Cadastrar"  

### ✅ Resultado Esperado
- Cadastro não deve ser efetuado  
- Exibir mensagem informando que o campo Senha é obrigatório  

### 📊 Resultado Obtido
- Cadastro não efetuado  
- Mensagem de campo Senha obrigatório exibida  

**Status:** ✅ Aprovado

---

## 📌 CT_CADASTRO_4 – Cadastrar com campo E-mail vazio

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Estar na página de cadastro |
| **Dados de Entrada** | Nome válido e senha válida |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja na página de cadastro  
- **Quando** deixar o campo E-mail vazio  
- **E** clicar em "Cadastrar"  

### ✅ Resultado Esperado
- Cadastro não deve ser efetuado  
- Exibir mensagem informando que o campo E-mail é obrigatório  

### 📊 Resultado Obtido
- Cadastro não efetuado  
- Mensagem de campo E-mail obrigatório exibida  

**Status:** ✅ Aprovado

---

## 📌 CT_CADASTRO_5 – Cadastrar com formato de E-mail inválido

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Estar na página de cadastro |
| **Dados de Entrada** | Nome e senha válidos; E-mail sem "@" |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja na página de cadastro  
- **Quando** informar um e-mail sem o caractere "@"  
- **E** clicar em "Cadastrar"  

### ✅ Resultado Esperado
- Cadastro não deve ser efetuado  
- Exibir mensagem informando que o formato do e-mail é inválido  

### 📊 Resultado Obtido
- Botão de cadastro permanece visível  
- Cadastro não realizado  

**Status:** ✅ Aprovado

---

## 📌 CT_CADASTRO_6 – Cadastro já existente

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Usuário já cadastrado no sistema |
| **Dados de Entrada** | Nome, e-mail e senha já existentes |

### 🧾 Passos (BDD)
- **Dado** que o usuário já esteja cadastrado  
- **Quando** tentar realizar um novo cadastro com os mesmos dados  
- **E** clicar em "Cadastrar"  

### ✅ Resultado Esperado
- Cadastro não deve ser efetuado  
- Exibir mensagem informando que o e-mail já está cadastrado  

### 📊 Resultado Obtido
- Mensagem de e-mail já cadastrado exibida  

**Status:** ✅ Aprovado

---

## 🧠 Observações
- Testes executados manualmente  
- Cenários focados em validações negativas e regras de negócio  
- Ambiente utilizado apenas para fins educacionais  

