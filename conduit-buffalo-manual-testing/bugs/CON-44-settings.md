# CON-44 — Settings recarrega a página inicial

## Ambiente
Windows com Ubuntu (WSL) e Google Chrome.
Buffalo executado localmente; PostgreSQL executado no Docker.
Endereço: http://127.0.0.1:3000

## Pré-condição
O usuário está conectado à sua conta.

## Passos para reproduzir
1. Abrir a página inicial.
2. Clicar em Settings no menu de navegação.

## Resultado obtido
A página inicial é recarregada e as configurações da conta não são abertas.
O usuário não consegue acessar a edição do perfil pelo link Settings.

## Resultado esperado
A página de configurações da conta é aberta e permite editar o perfil.

## Log do terminal
Após o clique em Settings, o terminal registra:
GET / — status 200

A requisição corresponde à página inicial, em vez de uma página de configurações.

## Evidências
- [Página após clicar em Settings](../evidence/settings-result.png)
- [Log do terminal](../evidence/terminal-log.png)

## Jira
Bug: CON-44
Story relacionada: CON-43
