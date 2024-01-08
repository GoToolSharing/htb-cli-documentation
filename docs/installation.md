# Installation

## Stable version

The **stable version (main branch)** of `htb-cli` only requires `golang version 20` to be installed (<a href="https://go.dev/doc/install" target="_blank">https://go.dev/doc/install</a>).

The following command downloads the binary :

```bash
go install github.com/GoToolSharing/htb-cli@latest
```

```bash
htb-cli version
Stable version (main branch): v1.5.1
```

Make sure you have golang in your **PATH** so you don't run into any problems when executing the binary. The following code must be added to your **rc file (bashrc / zshrc)** to make it permanent.

```bash
export GOPATH=$HOME/go
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
```

## Development version

The **development version (dev branch)** can be installed using the following command:

```bash
go install github.com/GoToolSharing/htb-cli@dev
```

```bash
htb-cli version
Development version (dev branch): a4cab218bb5f9851028091eb74469d4e21c469d0
```