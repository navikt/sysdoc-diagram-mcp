
## Prerequisites

### Graphviz

Graphviz is required to render diagrams. Install it with the package manager for your operating system:

```sh
# macOS (Homebrew)
brew install graphviz

# Debian/Ubuntu
sudo apt install graphviz

# Windows (winget)
winget install --id Graphviz.Graphviz -e
```

Verify that Graphviz is installed and `dot` is available on your `PATH`:

```sh
dot -V
```

If the command is not found after installation, restart your terminal and check that Graphviz is on your `PATH`.