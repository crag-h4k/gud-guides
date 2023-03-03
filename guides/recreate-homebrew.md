
# Recreate Homebrew environment in a new MacOS environment

## Install Homebrew

Run the command listend on Homebrew's [site](https://brew.sh/):

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Gather packages into a Brewfile (txt file)

1. Write all installed casks/formulae/images/taps into a Brewfile in the current
directory.

    ```sh
    brew bundle dump
    ```

2. Manually check that you want to install all the packages on your new system,
    remove unneeded packages

3. Install and upgrade (by default) all dependencies from the Brewfile - go get
a cold drink, this is will take a while

```sh
brew bundle
```
