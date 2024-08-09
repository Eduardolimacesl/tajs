# Commit Guide

1. Configurando [alias] em `~/.gitconfig`
```
[alias]
	unstage = reset HEAD --
	s = !git status -s 
	c = !git add --all && git commit -m 
	l = !git log --pretty=format:'%C(blue)%h %C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
```

2. 