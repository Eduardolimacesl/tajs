# Commit Guide

## Configurando [alias] em `~/.gitconfig`
Alias de `Rodrigo Manguinho`.
```
[alias]
	unstage = reset HEAD --
	s = !git status -s 
	c = !git add --all && git commit -m 
	l = !git log --pretty=format:'%C(blue)%h %C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
```
## Configurando um linter

1. Instala o commitlint (linter agnóstico de commits)
```shell
npm i -D @commitlint/cli@19.3.0
```
2. Instala o módulo conventional commits para o commitlint:
```shell
npm i -D @commitlint/config-conventional@19.2.2
```
3. Instalar o husky
```shell
npm i -D husky
``` 
---
## Commits
__Princípios:__

- ✅ Separe cada mudança lógica em um commit separado;
- ✅ Cada commit precisa ser justificável por seus próprios méritos - escopos isolados e vínculos com outros commits;
- ✅ Tempo verbal no `imperativo` no presente! Ex: "ajusta o bug"; "adiciona tal coisa"; O que esse commite faz com o projeto quando eu fizer o merge??
- 

### Tipos:

- build: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
- ci: Changes to our CI configuration files and scripts (example - scopes: Travis, Circle, BrowserStack, SauceLabs)
- docs: Documentation only changes
- feat: A new feature
- fix: A bug fix
- perf: A code change that improves performance
- refactor: A code change that neither fixes a bug nor adds a feature
- style: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- test: Adding missing tests or correcting existing tests

## Padrões de emojis 💈
[Emojis Github](https://gist.github.com/rxaviers/7360908?permalink_comment_id=5056224)

| Tipo do commit | Emoji | Palavra-chave |
| --- | --- | --- |
| Adicionando um teste | ✅ `:white_check_mark:` | `test` |
| Atualizando a versão de um submódulo | ⬆️ `:arrow_up:` |     |
| Retrocedendo a versão de um submódulo | ⬇️ `:arrow_down:` |     |
| Adicionando uma dependência | ➕ `:heavy_plus_sign:` | `build` |
| Alterações de revisão de código | 👌 `:ok_hand:` | `style` |
| Bugfix | 🐛 `:bug:` | `fix` |
| Comentários | 💡 `:bulb:` | `docs` |
| Commit inicial | 🎉 `:tada:` | `init` |
| Configuração | 🔧 `:wrench:` | `chore` |
| Deploy | 🚀 `:rocket:` |     |
| Documentação | 📚 `:books:` | `docs` |
| Em progresso | 🚧 `:construction:` |     |
| Estilização de interface | 💄 `:lipstick:` | `feat` |
| Infraestrutura | 🧱 `:bricks:` | `ci` |
| Lista de ideias (tasks) | 🔜 `:soon:` |     |
| Mover/Renomear | 🚚 `:truck:` | `chore` |
| Novo recurso | ✨ `:sparkles:` | `feat` |
| Package.json em JS | 📦 `:package:` | `build` |
| Performance | ⚡ `:zap:` | `perf` |
| Refatoração | ♻️ `:recycle:` | `refactor` |
| Limpeza de Código | 🧹 `:broom:` | `cleanup` |
| Removendo um arquivo | 🗑️ `:wastebasket:` | `remove` |
| Removendo uma dependência | ➖ `:heavy_minus_sign:` | `build` |
| Revertendo mudanças | 💥 `:boom:` | `fix` |
| Segurança | 🔒️ `:lock:` |     |
| SEO | 🔍️ `:mag:` |     |
| Tag de versão | 🔖 `:bookmark:` |     |
| Teste de aprovação | ✔️ `:heavy_check_mark:` | `test` |
| Testes | 🧪 `:test_tube:` | `test` |
| Texto | 📝 `:pencil:` |     |
| Tipagem | 🏷️ `:label:` |     |
| Tratamento de erros | 🥅 `:goal_net:` |     |
| Dados | 🗃️ `:card_file_box:` | `raw` |

## 💻 Exemplos
Padrão de commits [ConventionalCommits](https://www.conventionalcommits.org/en/v1.0.0/)

`:<emoji>: <type> (escopo opcional): <descrição>`

| Comando Git | Resultado no GitHub |
| --- | --- |
| `git commit -m ":tada: chore: Commit inicial"` | 🎉 chore: Commit inicial |
| `git commit -m ":books: docs: Atualização do README"` | 📚 docs: Atualização do README |
| `git commit -m ":bug: fix: Loop infinito na linha 50"` | 🐛 fix: Loop infinito na linha 50 |
| `git commit -m ":sparkles: feat: Página de login"` | ✨ feat: Página de login |
| `git commit -m ":bricks: ci: Modificação no Dockerfile"` | 🧱 ci: Modificação no Dockerfile |
| `git commit -m ":recycle: refactor: Passando para arrow functions"` | ♻️ refactor: Passando para arrow functions |
| `git commit -m ":zap: perf: Melhoria no tempo de resposta"` | ⚡ perf: Melhoria no tempo de resposta |
| `git commit -m ":boom: fix: Revertendo mudanças ineficientes"` | 💥 fix: Revertendo mudanças ineficientes |
| `git commit -m ":lipstick: feat: Estilização CSS do formulário"` | 💄 feat: Estilização CSS do formulário |
| `git commit -m ":test_tube: test: Criando novo teste"` | 🧪 test: Criando novo teste |
| `git commit -m ":bulb: docs: Comentários sobre a função LoremIpsum( )"` | 💡 docs: Comentários sobre a função LoremIpsum( ) |
| `git commit -m ":card_file_box: raw: RAW Data do ano aaaa"` | 🗃️ raw: RAW Data do ano aaaa |
| `git commit -m ":broom: cleanup: Eliminando blocos de código comentados e variáveis não utilizadas na função de validação de formulário"` | 🧹 cleanup: Eliminando blocos de código comentados e variáveis não utilizadas na função de validação de formulário |
| `git commit -m ":wastebasket: remove: Removendo arquivos não utilizados do projeto para manter a organização e atualização contínua"` | 🗑️ remove: Removendo arquivos não utilizados do projeto para manter a organização e atualização contínua |