# Plano de teste — Autenticação OrangeHRM

## 1. Objetivo

Verificar o comportamento funcional e aspectos básicos de usabilidade da autenticação do OrangeHRM, incluindo login, validações de entrada, uso do teclado e acesso à recuperação de senha.

## 2. Estratégia

Foram utilizados testes manuais funcionais, positivos, negativos e exploratórios. Os dados foram variados para observar o tratamento de letras maiúsculas e minúsculas, números, caracteres especiais, espaços, valores vazios e credenciais inválidas.

## 3. Critérios de entrada

- Aplicação demonstrativa disponível
- Tela de login acessível
- Credenciais públicas de demonstração disponíveis
- Navegador Google Chrome

## 4. Critérios de saída

- Casos planejados executados
- Resultados registrados
- Evidências coletadas para cenários representativos
- Comportamentos inesperados retestados antes da classificação como defeito

## 5. Riscos e limitações

- O ambiente é público e compartilhado, podendo sofrer alterações ou instabilidades.
- Não foi fornecida uma especificação formal dos requisitos.
- Os resultados representam o comportamento observado durante a execução.
- A execução foi realizada em apenas um navegador e sistema operacional.

## 6. Dados de teste

- Username válido: `Admin`
- Password válida: `admin123`
- Valores inválidos: `12345`, `@#$%`, `senha123`, espaços e campos vazios

