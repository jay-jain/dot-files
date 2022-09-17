# tmuxp

You can add a bash alias to call tmuxp:

```sh
alias split='if command -v tmux &> /dev/null && [ -n "$PS1" ] && [[ !"$TERM" =~ screen ]] && [[ ! "$TERM" =~ tmux ]] && [ -z "$TMUX" ]; then exec tmuxp load ~/.tmuxp/multiverse.yml; fi;'
```
