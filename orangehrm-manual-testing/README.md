# OrangeHRM — Testes manuais da autenticação

## Sobre o projeto

Este projeto apresenta a análise, elaboração e execução de testes manuais na área de autenticação do sistema demonstrativo OrangeHRM.

## Sistema testado

- **Aplicação:** OrangeHRM OS 5.9
- **URL:** https://opensource-demo.orangehrmlive.com/
- **Ambiente:** Google Chrome 153 / Windows 10
- **Data da execução:** 23/09/2026

## Escopo

- Tela de login
- Campos Username e Password
- Validação de credenciais
- Validação de campos obrigatórios
- Envio do formulário pelo botão Login e pela tecla Enter
- Navegação por teclado
- Link e tela de recuperação de senha

## Fora do escopo

- Funcionalidades internas após a autenticação
- Envio real de e-mail para redefinição de senha
- Testes de desempenho, carga e segurança aprofundada
- Compatibilidade com outros navegadores e dispositivos

## Documentação

- [Plano de teste](./test-plan.md)
- [Checklist](./checklist.md)
- [Casos de teste](./test-cases.md)
- [Resumo da execução](./test-summary.md)
- [Evidências](./evidence/)

## Resultado geral

Foram executados 19 casos de teste. Todos apresentaram o comportamento esperado. Durante o TC-003 ocorreu uma falha inicial de autenticação que não foi reproduzida no reteste; o fato foi mantido como observação, não como defeito confirmado.

