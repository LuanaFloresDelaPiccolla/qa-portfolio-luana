# Conduit — Testes de API com Postman

Autora: Luana Flores Dela Piccolla

Coleção criada durante os estudos de QA na Mate Academy. Testa um fluxo completo de registro, login, criação de artigo, criação de comentário e exclusão dos recursos criados.

## Cenários

| Ordem | Solicitação | Método | Endpoint | Status esperado | Testes |
| --- | --- | --- | --- | --- | --- |
| 1 | Registro | POST | users | 200 | Status e propriedades do usuário |
| 2 | Login | POST | users/login | 200 | Status, propriedades, e-mail e token |
| 3 | Criar um artigo | POST | articles | 200 | Status e propriedades do artigo e autor |
| 4 | Postar um comentário | POST | articles/{{slugConduit}}/comments | 200 | Status, propriedades e texto do comentário |
| 5 | Excluir um comentário | DELETE | articles/{{slugConduit}}/comments/{{commentId}} | 204 | Status |
| 6 | Excluir um artigo | DELETE | articles/{{slugConduit}} | 204 | Status |

## Como executar

1. Importe `conduit.postman_collection.json` no Postman.
2. Na coleção, abra Variables. BASE_URL já contém `https://conduit.mate.academy/api/`.
3. Preencha passwordConduit localmente com uma senha exclusiva para teste. Não publique seu valor.
4. Deixe No Environment selecionado para usar as variáveis da coleção.
5. Abra o Runner, selecione as seis solicitações na ordem da tabela e configure 3 iterações.
6. Execute a coleção.

O registro gera um novo usuário e e-mail usando {{$guid}} em cada execução. Os scripts salvam emailConduit, tokenConduit, slugConduit e commentId para as solicitações seguintes. Essas variáveis são preenchidas durante a execução; não precisam de valores iniciais.

## Resultado observado

Na execução realizada em 30/09/2026: 3 iterações, 30 testes aprovados, 0 falhas e 0 erros. Esse resultado refere-se à coleção original executada no Postman. A cópia deste repositório preserva as solicitações e os scripts e remove os valores salvos das variáveis, exceto BASE_URL; não foi executada novamente após a exportação.

## Ferramentas e conceitos

Postman, Chrome DevTools (Network), JavaScript, testes de status e response body, variáveis de coleção e encadeamento de solicitações.

A exclusão de artigo e comentário remove os recursos criados em cada iteração. As contas de teste criadas permanecem no aplicativo.
