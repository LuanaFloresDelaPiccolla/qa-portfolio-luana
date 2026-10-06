# Conduit — Postman Practice

Projeto de testes da API Conduit desenvolvido por Luana Flores.

## Cobertura

45 requisições com testes automatizados, organizadas em:

- User: 24 requisições
- Articles: 12 requisições
- Profile: 3 requisições
- Tags: 1 requisição
- Comments: 5 requisições

Os scripts de pré-requisição criam os dados necessários para cada cenário. Testes semelhantes reutilizam um auxiliar da coleção.

## Como executar

1. Importe o arquivo `.postman_collection.json` desta pasta no Postman.
2. Configure as variáveis da coleção:
   - `url`: `https://conduit.mate.academy/api`
   - `passwordConduit`: uma senha fictícia para os testes.
3. O script da coleção configura `testHelpers` automaticamente.
4. Execute todas as requisições no Collection Runner com uma iteração.

## Resultados

Na execução de 06/10/2026, somente User 09 e User 16 falharam nos testes. As falhas foram registradas no Jira:

- CON-41: cadastro aceita username com 41 caracteres.
- CON-42: cadastro aceita e-mail com 255 caracteres.

Nos dois casos, a API retornou 200 quando o esperado era 422. Os testes mantêm o resultado esperado para detectar os bugs.

## Ferramentas

Postman, JavaScript e Jira.
