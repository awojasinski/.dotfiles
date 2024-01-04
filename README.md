# dotfiles
Personal config files and all files needed to setup new machine.
To run setup script paste following command to your terminal

## requirements

### macOS

Following packages are required to correctly install dotfiles:
- Command Line Tools (CLT) for Xcode
- Homebrew

**Command Line Tools (CLT) for Xcode**

It contains tools for software development like git, compilers, python, etc. To install the package
paste following command into the terminal:

```bash
xcode-select --install
```

**Homebrew**

It's a free and open source package manager system used on macOS but can be also used on Linux.
the tool needs to have CLT for Xcode installed first. To install Homebrew execute following command
in the terminal:

```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## install

```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/awojasinski/.dotfiles/HEAD/bin/dotfiles)"
```
