# Matt's Dotfiles

## Adding Packages to GNU Stow

To add new package:

```shell
mkdir package/.config
```

Then add files to `package/.config`.

```shell
mv ~/.config/package package/.config/
```

## Installing Packages with GNU Stow

To install all packages:

```shell
stow *
```

To install specific package:

```shell
stow -vt ~ package
```

- `-v` verbose
- `-t` target directory

Dry run:

```shell
stow -nv package
```

- `-n` simulate
