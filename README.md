![CI status](https://github.com/awojasinski/.dotfiles/actions/workflows/playbook-lint.yml/badge.svg)

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

## usage

### install

```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/awojasinski/.dotfiles/HEAD/bin/dotfiles)"
```

## update

Run inside the repository:

```bash
./bin/dotfiles
```

This handles following operations:
- updates repository
- verify that all `ansible-galaxy` collections are updated
- run playbook from root directory of this repository

The command passes all arguments to the `ansible-playbook` command. This way you can pass arbitrary
arguments to the `ansible-playbook`. For instance if you would like to run only git role execute
following command:

```bash
./bin/dotfiles -t git
```