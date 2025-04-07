<h1><a name="top" title="dotfiles"></a><br/>~/.📁</h1>

<pre>
                _      _          
    |          | | o  | |         
  __|   __ _|_ | |    | |  _   ,  
 /  |  /  \_|  |/  |  |/  |/  / \_
 \_/|_/\__/ |_/|__/|_/|__/|__/ \/ 
               |\                 
               |/  by mina        

       ~ is where the ❤︎ is        
</pre>

<pre align="center">
Managed using <a href="https://www.chezmoi.io/">chezmoi</a>
</pre>

These are my personal dotfiles—the configuration files that help set up my systems exactly how I like them. They might not be perfect for you, but feel free to explore, copy, or adapt them for your own needs!

## quick start

To quickly install chezmoi and apply my dotfiles on a new machine, just run:

```sh
sh -c "$(curl -fsLS get.chezmoi.io)" -- init --apply minamarkham
```

Check out chezmoi's [Quick Start Guide](https://www.chezmoi.io/quick-start/) for more detailed instructions.

## usage

#### Update dotfiles

Pull and apply the latest changes:

```sh
chezmoi update -v
```

#### Add dotfiles

```sh
chezmoi add ~/.zshrc
```

#### Edit dotfiles

```sh
chezmoi edit ~/.zshrc
```

#### Preview changes

```sh
chezmoi diff
```

#### Apply changes

```sh
chezmoi -v apply
```

<div align="right"><sup><a href="#top">⬆ back to top</a></sup></div>

## what's inside
- `.aliases` – Shell command shortcuts.
- `.exports` – Environment variables.
- `.gitconfig` – Git preferences and aliases.
- `.gitignore.global` – Global Git ignores.
- `.path` – System `$PATH` configurations.
- `.starship.toml` – [Starship](https://starship.rs/) prompt settings.
- `.zprofile`, `.zshrc` – Zsh shell settings.

<div align="right"><sup><a href="#top">⬆ back to top</a></sup></div>

## customize

You can easily add your personal touches using the following files:

### `~/.zsh.local`

Automatically sourced after other shell files. Great for custom aliases or paths:

```sh
# Add custom paths
PATH="~/my/custom/path:$PATH"
export PATH

# Custom aliases
alias gs="git status"
```

### `~/.git.local`

Overrides or additional Git settings, ideal for sensitive information:

```gitconfig
[user]
  name = Your Name
  email = you@example.com
  signingKey = YOURGPGKEY
```

<div align="right"><sup><a href="#top">⬆ back to top</a></sup></div>

## license

The code is available under the [MIT license][license].

[license]: LICENSE
