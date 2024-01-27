# Hosts

!!! warning "Command in beta (v1)"

    The **hosts** command is a first version and may have **bugs** that could affect your `/etc/hosts` file. If it contains important information, I advise you to save it to avoid unpleasant surprises.

The **hosts** command lets the user interact with the `/etc/hosts` file to **add and remove** entries.

The `-a` / `--add` option specifies the domain to add.

The `-d` / `--delete` option specifies the domain to delete.

The `-i` / `--ip` option specifies the IP address associated with the domain.

```bash
htb-cli hosts -a git.machine.htb -i 10.10.10.10
```

![Add](/assets/commands/hosts/add.png)

```bash
htb-cli hosts -d dev.machine.htb -i 10.10.10.10
```

![Add](/assets/commands/hosts/delete.png)