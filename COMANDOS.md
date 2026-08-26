# Comandos de Git — Aula Git and GitHub for Beginners

## Comandos usados

| Comando | Função |
|---|---|
| `git branch` | Lista as branches locais e mostra qual está ativa (`*`) |
| `git checkout -b <nome>` | Cria uma branch nova e já muda para ela |
| `git checkout <nome>` | Muda para uma branch existente |
| `git diff` | Mostra diferenças não commitadas |
| `git diff <branch>` | Compara a branch atual com outra |
| `git branch -d <nome>` | Deleta uma branch (recusa se houver trabalho não mesclado) |
| `git commit -am "msg"` | Adiciona arquivos rastreados modificados + commita, em um passo |
| `git merge <branch>` | Mescla outra branch na branch atual |
| `git reset` | Desfaz stage |
| `git reset HEAD~1` | Volta 1 commit, mantém mudanças |
| `git reset --hard <hash>` | Volta a um commit específico, descarta tudo depois dele |
| `git log` | Histórico de commits com hashes |

## Comandos importantes que faltaram

| Comando | Função |
|---|---|
| `git stash` | Guarda mudanças não commitadas temporariamente, sem commitar |
| `git stash pop` | Recupera o que foi guardado no stash |
| `git clone <url>` | Copia um repositório remoto para a máquina local |
| `git fetch` | Baixa referências do remoto sem aplicar no código |

## Notas

- **git diff**: compara versões — sem argumento, compara working directory com staging.
- **-am**: `-a` adiciona arquivos já rastreados automaticamente; `-m` define a mensagem.
- **merge**: se as mudanças forem na mesma linha em branches diferentes, gera conflito.