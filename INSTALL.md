### [eza](https://github.com/eza-community/eza)

#### Install using Git

If you are a git user, you can install the theme and keep up to date by cloning the repo:

```bash
git clone https://github.com/urrickhunt/Dracula-for-eza.git
```

#### Install manually

Download using the [GitHub `.zip` download](https://github.com/urrickhunt/Dracula-for-eza/archive/refs/heads/main.zip) option and unzip them.

#### Activating theme

To activate the theme in **eza**, you need to modify your `.zshrc file`.

#### Installation

**Linux** & **macOS**

1. Add the desired `eza_colors` theme to the end of your `.zshrc`:

```zshrc
# ---------------------
# eza universal Dracula
# ---------------------
export EZA_COLORS="\
uu=36:\
uR=31:\
un=35:\
gu=37:\
da=2;34:\
ur=34:\
uw=95:\
ux=36:\
ue=36:\
gr=34:\
gw=35:\
gx=36:\
tr=34:\
tw=35:\
tx=36:\
xx=95:"
```

#### Suggested Aliases

For normal or larger displays include group (`-g flag`):

```zshrc
alias zl='eza -lagX --icons --color=always'
```

For smaller or limited displays no group:

```zshrc
alias zl='eza -laX --icons --color=always'
```

**Windows**

1. in either `Command Prompt` or `PowerShell` run the following with the windows universal eza theme:

   `setx EZA_WINDOWS_ATTRIBUTES "short"`

   `setx EZA_ICONS_AUTO "always"`

   `setx EZA_COLORS "da=2;34:xx=95:ur=36:su=95:sf=36:pi=96"`

2. Restart `Command Prompt` or `PowerShell`

#### Suggested Aliases

Add the following function to your PowerShell profile:

```ps1
function zl {
    eza -lagSX --icons --color=always --time-style=long-iso
}
```
