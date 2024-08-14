# ~/.dotfiles

<div align="center">

```
                _      _          
    |          | | o  | |         
  __|   __ _|_ | |    | |  _   ,  
 /  |  /  \_|  |/  |  |/  |/  / \_
 \_/|_/\__/ |_/|__/|_/|__/|__/ \/ 
               |\                 
               |/  by mina        
```

</div>

<pre align="center">
Managed using <a href="https://www.chezmoi.io/">chezmoi</a>
</pre>

This are my public dotfiles. These are config files to set up a system the way I like it. They might not work for you, but feel free to steal from them.

## Getting started

### Install chezmoi and the dotfiles on any new machine

With a single command:

```sh
chezmoi init --apply git@github.com:minamarkham/dotfiles.git
```

### Update

On any machine, you can pull and apply the latest changes from your repo with:

```sh
chezmoi update -v
```

### Add

```sh
chezmoi add ~/.zshrc
```

### Edit

```sh
chezmoi edit ~/.zshrc
```

### Preview

```sh
chezmoi diff
```

### Apply

```sh
chezmoi -v apply
```

## Synced Elsewhere
- Raycast
  - Cloud Sync
- Visual Studio Code
  - Settings Sync
- Hazel
  - Dropbox Sync
- Fonts
  - Fontbase/Dropbox

## License

The code is available under the [MIT license][license].

<!-- Link labels: -->
[license]: LICENSE
