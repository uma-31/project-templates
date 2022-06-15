# Project Templates

These are my project templates.

You can easily create a new project from template by using `clone-template`.

One feature of this command is that the new project is created as a local git repository,
and it contains only one commit history.

## Installation

### 1. Clone repository

```shell
$ git clone https://github.com/uma-31/project-templates.git "$HOME/.project-templates"
```

## 2. Install [gnu-getopt](https://formulae.brew.sh/formula/gnu-getopt) (Mac)

Here is a example of zsh.

```shell
$ brew install gnu-getopt
$ echo 'export PATH="/usr/local/opt/gnu-getopt/bin:$PATH"' >> ~/.zshrc
```

### 3. Set up your shell environment

Here is a example of zsh.

```shell
$ echo 'export PATH="$HOME/.project-templates:$PATH"' >> ~/.zshrc
```

### 4. Install `gh` (optional)

If you want to create remote repository automatically with `clone-template`,
you need to install `gh`.

See: https://github.com/cli/cli

### 5. Restart your shell

## Usage

```
clone-template [option] <template> <dest>

options:
  --create-repository       Create remote repository (GitHub).

  --repository-name <name>  Specify the name of the remote repository.

  --public                  Create public repository.
                            This option should be used with --create-repository.

  -h                        Display help.
```
