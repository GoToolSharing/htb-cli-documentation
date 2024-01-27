# Installation

## Stable version from remote

The **stable version (main branch)** of `htb-cli` only requires `golang version 20` to be installed (<a href="https://go.dev/doc/install" target="_blank">https://go.dev/doc/install</a>).

The following command downloads the binary :

```bash
go install github.com/GoToolSharing/htb-cli@latest
```

```bash
htb-cli version
Stable version (main branch): v1.6.0
```

Make sure you have golang in your **PATH** so you don't run into any problems when executing the binary. The following code must be added to your **rc file (bashrc / zshrc)** to make it permanent.

```bash
export GOPATH=$HOME/go
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
```

## Stable version from sources

```bash
git clone https://github.com/GoToolSharing/htb-cli.git
Cloning into 'htb-cli'...
remote: Enumerating objects: 1756, done.
remote: Counting objects: 100% (224/224), done.
remote: Compressing objects: 100% (131/131), done.
remote: Total 1756 (delta 106), reused 142 (delta 77), pack-reused 1532
Receiving objects: 100% (1756/1756), 4.21 MiB | 3.27 MiB/s, done.
Resolving deltas: 100% (1083/1083), done.
```

```bash
cd htb-cli
go install .
```

```bash
htb-cli version
Stable version (main branch): v1.6.0
```

## Development version from remote

The **development version (dev branch)** can be installed using the following command:

```bash
go install github.com/GoToolSharing/htb-cli@dev
```

```bash
htb-cli version
Development version (dev branch)
```

## Development version from sources

```bash
git clone https://github.com/GoToolSharing/htb-cli.git
Cloning into 'htb-cli'...
remote: Enumerating objects: 1756, done.
remote: Counting objects: 100% (224/224), done.
remote: Compressing objects: 100% (131/131), done.
remote: Total 1756 (delta 106), reused 142 (delta 77), pack-reused 1532
Receiving objects: 100% (1756/1756), 4.21 MiB | 3.27 MiB/s, done.
Resolving deltas: 100% (1083/1083), done.
```

```bash
cd htb-cli
git checkout dev
go install .
```

```bash
htb-cli version
Development version (dev branch)
```

## Pre-compiled binaries

**Pre-compiled binaries** are available with each release, allowing users to download the program without having to build it.

<a href="https://github.com/GoToolSharing/htb-cli/releases/tag/v1.6.0" target="_blank">https://github.com/GoToolSharing/htb-cli/releases/tag/v1.6.0</a>

![Binaries](/assets/configuration/binaries.png)
