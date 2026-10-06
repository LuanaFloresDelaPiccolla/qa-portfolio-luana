# Conduit API Testing — Postman

Projeto de testes da API Conduit desenvolvido por Luana Flores.

## Cobertura

45 requisições organizadas em cinco pastas:

- User: 24
- Articles: 12
- Profile: 3
- Tags: 1
- Comments: 5

As requisições incluem testes automatizados e criam os dados necessários nos scripts de pré-requisição. Testes de validação semelhantes reutilizam um auxiliar definido na coleção.

## Como executar

1. Importe o arquivo JSON desta pasta no Postman.
2. Nas variáveis da coleção, configure:
   - `url`: `https://conduit.mate.academy/api`
   - `passwordConduit`: uma senha fictícia para os usuários de teste.
3. O script de pré-requisição da coleção configura `testHelpers` automaticamente.
4. Execute a coleção no Collection Runner, com uma iteração e todas as requisições selecionadas.

## Resultado observado

Na execução realizada em 06/10/2026, somente as requisições User 09 e User 16 apresentaram falhas nos testes.

Bugs registrados no Jira:

- CON-41: cadastro aceita username com 41 caracteres.
- CON-42: cadastro aceita e-mail com 255 caracteres.

Esses testes esperam status 422, mas a API retornou 200. As expectativas foram mantidas para evidenciar os bugs.

## Ferramentas

Postman, JavaScript e Jira.
