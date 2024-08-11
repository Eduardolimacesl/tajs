# Commit Guide

## 1. Configurando [alias] em `~/.gitconfig`
```
[alias]
	unstage = reset HEAD --
	s = !git status -s 
	c = !git add --all && git commit -m 
	l = !git log --pretty=format:'%C(blue)%h %C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
```
---
## 2. Padrões de emojis 💈

| Tipo do commit | Emoji | Palavra-chave |
| --- | --- | --- |
| Acessibilidade | ♿ `:wheelchair:` |     |
| Adicionando um teste | ✅ `:white_check_mark:` | `test` |
| Atualizando a versão de um submódulo | ⬆️ `:arrow_up:` |     |
| Retrocedendo a versão de um submódulo | ⬇️ `:arrow_down:` |     |
| Adicionando uma dependência | ➕ `:heavy_plus_sign:` | `build` |
| Alterações de revisão de código | 👌 `:ok_hand:` | `style` |
| Animações e transições | 💫 `:dizzy:` |     |
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
| Responsividade | 📱 `:iphone:` |     |
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

## 3. 💻 Exemplos

| Comando Git | Resultado no GitHub |
| --- | --- |
| `git commit -m ":tada: Commit inicial"` | 🎉 Commit inicial |
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