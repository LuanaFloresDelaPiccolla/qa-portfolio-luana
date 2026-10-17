# Huntd — Testes manuais web e iOS

Projeto de estudo de **Luana Flores**, desenvolvido durante o curso de Quality Assurance da **Mate academy**. O Huntd é uma plataforma de recrutamento com perfis de candidatos e recrutadores.

O trabalho reúne planejamento, decomposição funcional, casos de teste, matriz de rastreabilidade, permissões e relatos de bugs em desktop, navegador mobile e aplicativo iOS.

## Resultados registrados

| Ambiente | Passed | Failed | Blocked | Total de registros |
| --- | ---: | ---: | ---: | ---: |
| Chrome desktop | 20 | 12 | 0 | 32 |
| Safari no iPhone | 22 | 7 | 3 | 32 |
| Aplicativo iOS | 5 | 3 | 6 | 14 |

**46 casos agrupados e 16 bugs únicos documentados.** Os 32 casos web foram reutilizados em Chrome e Safari. Bloqueios estão incluídos na tabela. Consulte a [interpretação dos resultados e limitações](results.md) antes de comparar os números.

## Documentação

| Arquivo | Conteúdo |
| --- | --- |
| [Plano de testes](test-plan.md) | Objetivo, escopo, abordagem e critérios |
| [Resultados](results.md) | Resumo por ambiente e limites da análise |
| [Casos web](web-test-cases.csv) | 32 casos agrupados com status por navegador |
| [Casos iOS](ios-test-cases.csv) | 14 casos agrupados com status registrado |
| [Bugs detalhados](bugs.md) | Pré-condições, passos e resultados de 16 relatos |
| [Registro de bugs](bug-register.csv) | Lista para consulta e filtros |
| [Decomposição web](web-decomposition.csv) / [iOS](ios-decomposition.csv) | Funcionalidades e pontos de verificação |
| [RTM web](web-rtm.csv) / [iOS](ios-rtm.csv) | Relações entre requisitos, casos e histórias |
| [Permissões](permission-table.csv) | Comportamento esperado por perfil; não é uma validação concluída |

## Exemplos de problemas registrados

- Busca de localização sem opções, impedindo continuar o cadastro no iOS (HUNT-3).
- Filtro de tecnologia que limpa a seleção sem aplicá-la (HUNT-25).
- Campos de perfil apagados ao voltar da etapa seguinte no iOS (HUNT-22).
- E-mail de recuperação não recebido durante a verificação (HUNT-21 e HUNT-29).

## Ferramentas e prática

**Jira, TestRail e planilhas.** Planejamento e priorização, cenários positivos e negativos, testes exploratórios, registro de defeitos e rastreabilidade. Os documentos podem ser lidos diretamente no GitHub; não exigem acesso às contas do curso.

Esta versão apresenta registros históricos de outubro de 2026. Não confirma o comportamento atual do produto nem inclui anexos de evidências. IDs foram preservados, sem credenciais, links privados de execução ou dados de candidatos. O relatório original permanece separado desta edição pública.

**Autora:** Luana Flores · estudante de Quality Assurance.
