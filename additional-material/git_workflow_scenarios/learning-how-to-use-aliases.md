

# Git Aliases for Beginners

## Setting Up Git Aliases

To set up a Git alias, you use the `git config` command. Aliases are stored in your Git configuration file, which can be global (for all repositories) or local (for a specific repository).

### Creating Global Aliases

To create an alias that works in all repositories, use the `--global` option:

```sh
git config --global alias.<alias-name> '<git-command>'
```

### Creating Local Aliases

To create an alias that works only in the current repository, omit the `--global` option:

```sh
git config alias.<alias-name> '<git-command>'
```

## Common Git Aliases

### Status

Instead of typing `git status`, you can create a shorter alias:

```sh
git config --global alias.st 'status'
```

### Log

For a more readable log format, you can set up an alias:

```sh
git config --global alias.lg 'log --oneline --graph --decorate --all'
```

### Commit

Shorten the commit command:

```sh
git config --global alias.ci 'commit'
```

### Checkout

For faster branch switching:

```sh
git config --global alias.co 'checkout'
```

### Branch

To list all branches:

```sh
git config --global alias.br 'branch'
```
