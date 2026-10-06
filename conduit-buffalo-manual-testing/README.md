# Conduit Buffalo — Testes Manuais

Prática de testes manuais realizada por Luana Da Silva Flores em 6 de outubro de 2026.

## Objetivo
Executar a aplicação localmente, investigar falhas e documentar os resultados com prints e logs do terminal.

## Ambiente
- Windows com Ubuntu (WSL)
- Google Chrome
- Aplicação Buffalo executada localmente com `buffalo dev`
- PostgreSQL executado em um container Docker
- Endereço: http://127.0.0.1:3000

## Testes realizados
- Cadastro de usuário realizado com sucesso.
- Verificação da navegação para as configurações da conta.
- Verificação da apresentação visual das páginas.
- Análise dos logs do terminal e das respostas na aba Network.

## Bugs encontrados
- [CON-44: Settings não abre as configurações](bugs/CON-44-settings.md)
- [CON-45: Página sem formatação por falha no carregamento do CSS](bugs/CON-45-missing-css.md)

Os dois bugs foram vinculados à Story CON-43 no Jira.

## Arquivos
- `bugs/`: relatórios com passos de reprodução e resultados.
- `evidence/`: prints das páginas, logs e respostas HTTP.

## Escopo
Esta atividade foi uma sessão focada de testes exploratórios. Não representa um teste de regressão completo da aplicação.
