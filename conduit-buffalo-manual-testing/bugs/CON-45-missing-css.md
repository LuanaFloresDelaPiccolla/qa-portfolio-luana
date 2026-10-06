# CON-45 — Páginas da aplicação sem formatação

## Ambiente
Windows com Ubuntu (WSL) e Google Chrome.
Buffalo executado localmente; PostgreSQL executado no Docker.
Endereço: http://127.0.0.1:3000

## Passos para reproduzir
1. Abrir a aplicação.
2. Observar a apresentação visual da página.
3. Verificar os logs do terminal e a aba Network do navegador.

## Resultado obtido
A página exibe HTML sem a formatação esperada.
Os arquivos locais buffalo.css e application.css retornam 404.
O arquivo externo https://demo.productionready.io/main.css também retorna 404.

## Resultado esperado
Os arquivos CSS são carregados com sucesso e a página apresenta o layout e a formatação previstos.

## Trechos dos logs do terminal
Trechos transcritos do print do terminal:

could not find assets/buffalo.css status=404
could not find assets/application.css status=404

## Evidência do navegador
A aba Network mostra uma requisição GET para:
https://demo.productionready.io/main.css

Resposta: 404 Not Found.

## Evidências
- [Página sem formatação](../evidence/settings-result.png)
- [Erros no terminal](../evidence/terminal-log.png)
- [Resposta 404 do CSS externo](../evidence/main-css-404.png)

## Jira
Bug: CON-45
Story relacionada: CON-43
