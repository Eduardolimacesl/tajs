# Método Testes Automatizados utilizando JavaScript (TAJS)

Método que estabelece uma métrica de qualidade e uma organização mental para o desenvolvimento basedo no TDD(Test Driven Development)

## Pilares
> Não tocar no código enquanto você não estiver **100% satisfeito** que entendeu o problema e *o passo a passo* para a *solução*.
---
Criar um notebook (tabela) com os 3 campos:
- **ENTRADA**: O que é preciso de informação para executar uma função?
- **PROCESSAMENTO**: O que eu faço com esses dados?
- **SAÍDA**: O que essa função deve retornar?
Fazer uma dupla validação para apresentar o que foi entendido dos requisitos!
---
> Valide o que vc entregou de forma automatizada. Escrever todos os caminhos da aplicação para uma funcionalidade específica:
---
- Cenário de Sucesso:
  - Entrada
  - Saída
- Cenário de erro:
  - Entrada
  - Saída
- Cenário Alternativo:
  - Entrada
  - Saída
---
> Prepare o Setup fundamental (teste e debbuging) no momento da criação do Projeto
---

## Setup padrão
Setup com o livereload ativado.

1. Na pasta de trabalho iniciar o módulo utilizando o `package.json`
```shell
npm init -y
npm pkg set type=module engines.node=$(node -v) author=eduardolimacesl  
```

2. Instalando o Jest:
```shell
npm i -D jest@29
npx jest --init
```
3. Instalando o ntl
```shell
npm i -g ntl
```
## Conceitos
