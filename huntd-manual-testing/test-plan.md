# Plano de testes

## Objetivo

Verificar funcionalidades e permissões da plataforma de recrutamento Huntd em desktop, navegador mobile e aplicativo iOS, conforme os requisitos do exercício da Mate academy.

## Escopo

- Web: páginas públicas, cadastro e login, recuperação de senha, perfis de candidatos e recrutadores, filtros, chats, empresas, vagas e navegação.
- iOS: autenticação, cadastro, perfis, chats, preferências e navegação implementada.
- Perfis de acesso: visitante, candidato e recrutador.

## Abordagem

Testes manuais funcionais, exploratórios, de interface, responsividade e permissões. Cenários positivos e negativos, com partições de equivalência e valores-limite previstos no plano de origem. Prioridade para autenticação, criação de perfil, permissões e chats.

Ferramentas: TestRail para casos e resultados, Jira para histórias e bugs e planilha para planejamento, rastreabilidade e resumo.

## Dados e ambientes

Contas de teste separadas para candidato e recrutador, dados fictícios e variações válidas e inválidas. Nenhuma credencial faz parte deste portfólio. Ambientes registrados: Chrome no Windows, Safari no iPhone e aplicativo Huntd para iOS. Veja versões e limitações em [Resultados](results.md).

## Critérios e bloqueios

Entrada: requisitos disponíveis, acesso à aplicação, contas de teste e casos preparados. Saída planejada: verificações executáveis registradas, falhas e bloqueios documentados, bugs rastreáveis e resumo atualizado. A existência de bloqueios impede afirmar validação integral do escopo.

Continuar com os recursos acessíveis quando ativação de conta, localização, e-mail, integração externa ou falta de dados controlados impedir um cenário. Registrar o motivo e retomar após resolver a dependência.

## Fora do escopo

Administração, formulário de perguntas/feedback e recursos não implementados no aplicativo. Este repositório não apresenta testes automatizados, de carga ou uma avaliação de segurança.

## Fonte e autoria

Exercício Huntd da Mate academy e relatório final de Luana Flores, com resultados datados de 10/10/2026. A documentação pública foi organizada em 17/10/2026 sem nova execução. A duração estimada de planejamento não é apresentada como horas efetivamente trabalhadas.
