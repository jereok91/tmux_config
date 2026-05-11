# Configuracion de tmux

Esta configuracion usa TPM (Tmux Plugin Manager) y plugins declarados en `.tmux.conf`.

## Requisitos

- `tmux` instalado
- `git` instalado

## Instalacion

1) Coloca el archivo `.tmux.conf` en tu HOME:

```sh
cp /ruta/a/este/repo/.tmux.conf ~/.tmux.conf
```

2) Crea la carpeta de plugins y clona TPM:

```sh
mkdir -p ~/.tmux/plugins
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

3) Recarga la configuracion en tmux:

```sh
tmux source-file ~/.tmux.conf
```

4) Instala los plugins desde tmux:

- Presiona `prefix + I` (por defecto `prefix` es `Ctrl-a`).

Los plugins se instalaran en `~/.tmux/plugins`.

## Plugins incluidos

- tmux-plugins/tpm
- tmux-plugins/tmux-sensible
- tmux-plugins/tmux-yank
- christoomey/vim-tmux-navigator
- tmux-plugins/tmux-resurrect
- alexwforsythe/tmux-which-key
- Nybkox/tmux-ukiyo

## Notas

- En Linux se usa `clip` para copiar desde el modo copy.
- En macOS se usa `pbcopy`.
