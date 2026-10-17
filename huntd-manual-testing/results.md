# Resultados e limitações

Data dos resultados: **10/10/2026**. Fonte: colunas de status do relatório final de estudo. Nenhum teste foi executado novamente para preparar este portfólio.

| Ambiente | Passed | Failed | Blocked | Total de registros |
| --- | ---: | ---: | ---: | ---: |
| Chrome desktop | 20 | 12 | 0 | 32 |
| Safari no iPhone | 22 | 7 | 3 | 32 |
| Aplicativo iOS | 5 | 3 | 6 | 14 |

São **46 casos agrupados**: 32 web reutilizados em dois navegadores e 14 iOS. A matriz contém **78 registros de resultado**, incluindo os bloqueados. Esses números não significam 78 casos únicos nem 78 execuções concluídas com sucesso.

## Como interpretar

- Passed: resultado aprovado registrado no caso agrupado.
- Failed: caso agrupado com falha registrada.
- Blocked: parte necessária não pôde ser validada.
- Um caso agrupa várias verificações. Um resultado agregado pode coexistir com variações bloqueadas nas anotações originais; ele não comprova aprovação de todas as variações.
- Os 16 IDs de bugs únicos não devem ser somados às 22 falhas da matriz: uma falha pode afetar mais de um ambiente ou caso.

## Limitações da documentação de origem

A planilha final mantém notas de planejamento antigas, referências a abas de histórico ausentes e mensagens de pendência que não acompanham as colunas finais. Por isso, os CSVs públicos preservam os status registrados e não reproduzem notas antigas como se fossem o estado atual. Não foi feita uma conciliação com os resultados individuais no TestRail.

Os ambientes e versões foram informados durante o estudo. Windows 10 Pro 22H2 e Chrome 154.0.8037.98 foram registrados para desktop; iPhone 15 Plus, iOS 26.6.2 e Huntd 1.2.6.22 para mobile. Não foram reconfirmados nesta preparação.

A tabela de permissões descreve comportamento esperado, com validações pendentes. Os arquivos RTM relacionam requisitos e casos; não constituem prova de cobertura integral.

Evidências em vídeo e imagens não foram anexadas à versão pública. Os relatos de bugs mantêm passos e resultados, mas os anexos no Jira não foram conferidos nesta preparação. A ausência do e-mail de recuperação registra uma observação, sem determinar a causa. O erro 500 foi relatado visualmente, sem confirmação de status HTTP no Network.

Algumas divergências dependem dos requisitos do exercício, como a ordem das experiências, a quantidade de depoimentos e os links sociais. Não representam necessariamente defeitos segundo as regras atuais do produto.
