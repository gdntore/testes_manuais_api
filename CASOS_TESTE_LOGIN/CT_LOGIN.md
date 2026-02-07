# 🧪 Casos de Teste – Login (ServeRest)

**Projeto:** Portfólio QA  
**Tipo de Teste:** Testes Funcionais / Testes Manuais  
**Sistema:** https://front.serverest.dev/login  
**Navegadores:** Google Chrome | Brave | Firefox  

---

## 📌 CT_LOGIN_1 – Campos vazios

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Estar na página de login |
| **Dados de Entrada** | N/A |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja na página de login  
- **Quando** deixar os campos de e-mail e senha vazios  
- **E** clicar no botão "Entrar"  

### ✅ Resultado Esperado
- Login não deve ser efetuado  
- Exibir mensagem informando que o e-mail e a senha são obrigatórios  

### 📊 Resultado Obtido
- Mensagem exibida:  
  - Email é obrigatório  
  - Password é obrigatório  

**Status:** ✅ Aprovado

---

## 📌 CT_LOGIN_2 – E-mail válido e senha inválida

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Estar na página de login |
| **Dados de Entrada** | E-mail válido e senha inválida |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja na página de login  
- **Quando** inserir um e-mail válido  
- **E** inserir uma senha incorreta  
- **E** clicar no botão "Entrar"  

### ✅ Resultado Esperado
- Login não deve ser efetuado  
- Exibir mensagem informando que o e-mail e/ou senha são inválidos  

### 📊 Resultado Obtido
- Mensagem exibida: Email e/ou senha inválidos  

**Status:** ✅ Aprovado

---

## 📌 CT_LOGIN_3 – E-mail inválido e senha válida

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Estar na página de login |
| **Dados de Entrada** | E-mail sem "@" e senha válida |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja na página de login  
- **Quando** inserir um e-mail sem o caractere "@"  
- **E** inserir uma senha válida  
- **E** clicar no botão "Entrar"  

### ✅ Resultado Esperado
- Login não deve ser efetuado  
- Exibir mensagem informando que o formato do e-mail é inválido  

### 📊 Resultado Obtido
- Mensagem exibida informando ausência do caractere "@" no e-mail  

**Status:** ✅ Aprovado

---

## 📌 CT_LOGIN_4 – E-mail e senha válidos

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Estar na página de login; Possuir cadastro válido |
| **Dados de Entrada** | E-mail e senha válidos |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja na página de login  
- **Quando** inserir um e-mail válido  
- **E** inserir uma senha válida  
- **E** clicar no botão "Entrar"  

### ✅ Resultado Esperado
- Login deve ser efetuado com sucesso  
- Usuário deve ser redirecionado para a página principal  

### 📊 Resultado Obtido
- Login realizado com sucesso  
- Página principal exibida  

**Status:** ✅ Aprovado

---

## 📌 CT_LOGIN_5 – Botão "Entrar" sem preenchimento dos campos

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Estar na página de login |
| **Dados de Entrada** | N/A |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja na página de login  
- **Quando** não preencher o e-mail  
- **E** não preencher a senha  

### ✅ Resultado Esperado
- Botão "Entrar" não deve permitir ação de login  

### 📊 Resultado Obtido
- Botão permanece visível mesmo sem preenchimento dos campos  

**Status:** ✅ Aprovado

---

## 📌 CT_LOGIN_6 – Redirecionamento para cadastro

| Campo | Descrição |
|------|----------|
| **Prioridade** | Alta |
| **Pré-condições** | Estar na página de login |
| **Dados de Entrada** | N/A |

### 🧾 Passos (BDD)
- **Dado** que o usuário esteja na página de login  
- **Quando** clicar no botão "Cadastre-se"  

### ✅ Resultado Esperado
- Usuário deve ser redirecionado para a página de cadastro  

### 📊 Resultado Obtido
- Página de cadastro exibida com sucesso  

**Status:** ✅ Aprovado

---

## 🧠 Observações
- Testes executados manualmente  
- Cenários focados em validações funcionais e regras de negócio  
- Ambiente utilizado apenas para fins educacionais  

