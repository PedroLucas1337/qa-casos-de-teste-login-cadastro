# Casos de Teste – Funcionalidades de Login e Cadastro

## Objetivo Geral
Detalhar de forma clara todas as **8 funcionalidades de Login e Cadastro**, visando a melhor usabilidade e contemplando:
- Cenários positivos e negativos
- Duplicidade de dados
- Falta de campos obrigatórios
- Campos inválidos e/ou inexistentes

---

## Passos Comuns (PCs)

- **PC-01** – Acessar a página correspondente (Login ou Cadastro)  
- **PC-02** – Preencher corretamente os campos não relacionados ao cenário  
- **PC-03** – Submeter o formulário  

---

## ID 1 – Cadastro com campos vazios (Nome, Email)

### 1.1 – Tentar cadastrar com campo **Nome** vazio
**Objetivo:** Verificar se o sistema bloqueia o cadastro de usuários com o campo “Nome” vazio.

**Pré-condições:**
- Usuário não estar autenticado  
- Página de Cadastro estar disponível  

**Passos:**
1. PC-01  
2. Deixar o campo obrigatório **Nome** vazio  
3. PC-02  
4. PC-03  

**Resultado Esperado:**  
O cadastro é barrado com um alerta informando:  
> “O campo nome é obrigatório para o cadastro.”

---

### 1.2 – Tentar cadastrar com campo **Email** vazio
**Objetivo:** Verificar se o sistema bloqueia o cadastro de usuários com o campo “Email” vazio.

**Pré-condições:**
- Usuário não estar autenticado  
- Página de Cadastro estar disponível  

**Passos:**
1. PC-01  
2. Deixar o campo obrigatório **Email** vazio  
3. PC-02  
4. PC-03  

**Resultado Esperado:**  
O cadastro é barrado com um alerta informando:  
> “O campo email é obrigatório para o cadastro.”

---

## ID 2 – Cadastro com campos inválidos

### 2.1 – Registrar senha fraca
**Objetivo:** Verificar se o sistema bloqueia senhas consideradas fracas.

**Pré-condições:**
- Usuário não estar autenticado  
- Página de Cadastro estar disponível  

**Passos:**
1. PC-01  
2. Inserir senha fraca (ex: `123456`)  
3. PC-02  
4. PC-03  

**Resultado Esperado:**  
Cadastro barrado com alerta:  
> “A senha é muito fraca. Utilize letras, números e caracteres especiais.”

---

### 2.2 – Registrar email inválido
**Objetivo:** Verificar se o sistema reconhece emails inválidos.

**Pré-condições:**
- Usuário não estar autenticado  
- Página de Cadastro estar disponível  

**Passos:**
1. PC-01  
2. Inserir email inválido (ex: `pedro@.com`)  
3. PC-02  
4. PC-03  

**Resultado Esperado:**  
Cadastro barrado com alerta:  
> “O email informado é inválido. Utilize o formato nome@dominio.com.”

---

## ID 3 – Cadastro com dados já existentes

### 3.1 – Email já cadastrado
**Objetivo:** Verificar se o sistema bloqueia emails duplicados.

**Pré-condições:**
- Email `pedrolucas@gmail.com` já cadastrado  

**Passos:**
1. PC-01  
2. Inserir email já existente  
3. PC-02  
4. PC-03  

**Resultado Esperado:**  
Cadastro barrado com alerta:  
> “Este email já está cadastrado. Por favor, utilize outro.”

---

### 3.2 – CPF já cadastrado
**Objetivo:** Verificar se o sistema bloqueia CPFs duplicados.

**Pré-condições:**
- CPF `999.999.999-99` já cadastrado  

**Passos:**
1. PC-01  
2. Inserir CPF já existente  
3. PC-02  
4. PC-03  

**Resultado Esperado:**  
Cadastro barrado com alerta:  
> “Este CPF já está cadastrado. Por favor, utilize outro.”

---

## ID 4 – Cadastro com dados válidos

### 4.1 – Cadastro bem-sucedido
**Objetivo:** Validar cadastro com dados válidos e redirecionamento para login.

**Pré-condições:**
- Usuário não estar autenticado  
- Página de Cadastro acessível  

**Passos:**
1. PC-01  
2. PC-02  
3. PC-03  

**Resultado Esperado:**  
Mensagem de sucesso exibida e redirecionamento para a tela de login.

---

## ID 5 – Login com campos vazios

### 5.1 – Login sem usuário
**Objetivo:** Verificar se o sistema bloqueia login sem usuário.

**Pré-condições:**
- Usuário não estar autenticado  
- Página de Login acessível  

**Passos:**
1. PC-01  
2. Deixar campo **Usuário** vazio  
3. PC-02  
4. PC-03  

**Resultado Esperado:**  
Login barrado com alerta informando campo obrigatório.

---

### 5.2 – Login sem senha
**Objetivo:** Verificar se o sistema bloqueia login sem senha.

**Pré-condições:**
- Usuário não estar autenticado  
- Página de Login acessível  

**Passos:**
1. PC-01  
2. Deixar campo **Senha** vazio  
3. PC-02  
4. PC-03  

**Resultado Esperado:**  
Login barrado com alerta informando campo obrigatório.

---

## ID 6 – Login com dados inválidos

### 6.1 – Usuário inexistente
**Objetivo:** Validar bloqueio de usuário inexistente.

**Pré-condições:**
- Usuário não estar autenticado  

**Passos:**
1. PC-01  
2. Inserir usuário inexistente  
3. PC-02  
4. PC-03  

**Resultado Esperado:**  
Login barrado com alerta de usuário inexistente.

---

### 6.2 – Senha inválida
**Objetivo:** Validar bloqueio de senha incorreta.

**Pré-condições:**
- Usuário não estar autenticado  

**Passos:**
1. PC-01  
2. Inserir senha inválida  
3. PC-02  
4. PC-03  

**Resultado Esperado:**  
Login barrado com alerta de senha inválida.

---

## ID 7 – Esqueceu a Senha

### 7.1 – Funcionamento do botão
**Objetivo:** Verificar redirecionamento correto para recuperação de senha.

**Pré-condições:**
- Usuário não estar autenticado  
- Página de Login acessível  

**Passos:**
1. PC-01  
2. Clicar em **Esqueceu a senha**  

**Resultado Esperado:**  
Usuário redirecionado para a tela de recuperação de senha.

---

## ID 8 – Login com credenciais válidas

### 8.1 – Login bem-sucedido
**Objetivo:** Validar login com dados válidos.

**Pré-condições:**
- Usuário não estar autenticado  
- Usuário possuir cadastro válido  

**Passos:**
1. PC-01  
2. PC-02  
3. PC-03  

**Resultado Esperado:**  
Usuário autenticado e redirecionado para a página inicial.
