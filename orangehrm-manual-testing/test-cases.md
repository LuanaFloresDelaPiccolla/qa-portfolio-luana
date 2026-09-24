# Casos de teste — Autenticação OrangeHRM

## TC-001 — Login com credenciais válidas

- **Dados:** Username `Admin`; Password `admin123`
- **Ação:** clicar em Login
- **Resultado esperado:** acesso ao sistema
- **Resultado obtido:** acesso realizado com sucesso
- **Status:** Passed

## TC-002 — Login com Username em letras minúsculas

- **Dados:** Username `admin`; Password `admin123`
- **Ação:** clicar em Login
- **Resultado esperado:** verificar o tratamento da capitalização do Username
- **Resultado obtido:** acesso realizado com sucesso
- **Status:** Passed

## TC-003 — Login com Username em letras maiúsculas

- **Dados:** Username `ADMIN`; Password `admin123`
- **Ação:** clicar em Login e repetir a execução após a falha inicial
- **Resultado esperado:** verificar o tratamento da capitalização do Username
- **Resultado obtido:** acesso realizado no reteste
- **Status:** Passed
- **Observação:** a primeira tentativa exibiu `Invalid credentials`, mas o comportamento não foi reproduzido no reteste

## TC-004 — Login com Username numérico

- **Dados:** Username `12345`; Password `admin123`
- **Ação:** clicar em Login
- **Resultado esperado:** acesso negado
- **Resultado obtido:** mensagem `Invalid credentials`
- **Status:** Passed

## TC-005 — Login com caracteres especiais no Username

- **Dados:** Username `@#$%`; Password `admin123`
- **Ação:** clicar em Login
- **Resultado esperado:** acesso negado
- **Resultado obtido:** mensagem `Invalid credentials`
- **Status:** Passed

## TC-006 — Login com os dois campos vazios

- **Dados:** Username vazio; Password vazia
- **Ação:** clicar em Login
- **Resultado esperado:** impedir o acesso e indicar os campos obrigatórios
- **Resultado obtido:** mensagem `Required` abaixo dos dois campos e bordas vermelhas
- **Status:** Passed
- **Evidência:** [TC-006-empty-fields.png](./evidence/TC-006-empty-fields.png)

## TC-007 — Login com Username vazio

- **Dados:** Username vazio; Password `admin123`
- **Ação:** clicar em Login
- **Resultado esperado:** impedir o acesso e indicar que Username é obrigatório
- **Resultado obtido:** mensagem `Required` e borda vermelha somente no Username
- **Status:** Passed
- **Evidência:** [TC-007-empty-username.png](./evidence/TC-007-empty-username.png)

## TC-008 — Login com Password vazio

- **Dados:** Username `Admin`; Password vazia
- **Ação:** clicar em Login
- **Resultado esperado:** impedir o acesso e indicar que Password é obrigatório
- **Resultado obtido:** mensagem `Required` e borda vermelha somente no Password
- **Status:** Passed

## TC-009 — Username preenchido somente com espaços

- **Dados:** Username com três espaços; Password `admin123`
- **Ação:** clicar em Login
- **Resultado esperado:** considerar o Username vazio e impedir o acesso
- **Resultado obtido:** mensagem `Required` no Username
- **Status:** Passed

## TC-010 — Espaços antes e depois do Username válido

- **Dados:** Username `   Admin   `; Password `admin123`
- **Ação:** clicar em Login
- **Resultado esperado:** acesso negado para credencial diferente da cadastrada
- **Resultado obtido:** mensagem `Invalid credentials`
- **Status:** Passed

## TC-011 — Login com senha incorreta

- **Dados:** Username `Admin`; Password `senha123`
- **Ação:** clicar em Login
- **Resultado esperado:** acesso negado
- **Resultado obtido:** mensagem `Invalid credentials`
- **Status:** Passed

## TC-012 — Login com senha em letras maiúsculas

- **Dados:** Username `Admin`; Password `ADMIN123`
- **Ação:** clicar em Login
- **Resultado esperado:** acesso negado porque a senha diferencia maiúsculas e minúsculas
- **Resultado obtido:** mensagem `Invalid credentials`
- **Status:** Passed

## TC-013 — Espaços antes e depois da senha válida

- **Dados:** Username `Admin`; Password `   admin123   `
- **Ação:** clicar em Login
- **Resultado esperado:** acesso negado para credencial diferente da cadastrada
- **Resultado obtido:** mensagem `Invalid credentials`
- **Status:** Passed

## TC-014 — Login utilizando a tecla Enter

- **Dados:** Username `Admin`; Password `admin123`
- **Ação:** pressionar Enter após preencher as credenciais
- **Resultado esperado:** enviar o formulário e acessar o sistema
- **Resultado obtido:** acesso realizado com sucesso
- **Status:** Passed

## TC-015 — Acessar a recuperação de senha

- **Pré-condição:** usuário na tela de login
- **Ação:** clicar em Forgot your password?
- **Resultado esperado:** abrir a página de recuperação de senha
- **Resultado obtido:** página Reset Password aberta com campo Username e botões Cancel e Reset Password
- **Status:** Passed

## TC-016 — Cancelar a recuperação de senha

- **Pré-condição:** usuário na página Reset Password
- **Ação:** clicar em Cancel
- **Resultado esperado:** retornar para a tela de login
- **Resultado obtido:** tela de login aberta e URL finalizada em `/auth/login`
- **Status:** Passed

## TC-017 — Recuperação de senha com Username vazio

- **Pré-condição:** usuário na página Reset Password
- **Dados:** Username vazio
- **Ação:** clicar em Reset Password
- **Resultado esperado:** impedir o envio e indicar que Username é obrigatório
- **Resultado obtido:** mensagem `Required` no campo Username
- **Status:** Passed

## TC-018 — Mascaramento da senha

- **Ação:** digitar uma senha no campo Password
- **Resultado esperado:** ocultar os caracteres da senha
- **Resultado obtido:** caracteres representados por pontos
- **Status:** Passed
- **Evidência:** [TC-007-empty-username.png](./evidence/TC-007-empty-username.png)

## TC-019 — Navegação utilizando a tecla Tab

- **Pré-condição:** usuário na tela de login
- **Ação:** posicionar o foco em Username e pressionar Tab duas vezes
- **Resultado esperado:** seguir a ordem Username → Password → Login
- **Resultado obtido:** navegação realizada na ordem esperada
- **Status:** Passed

