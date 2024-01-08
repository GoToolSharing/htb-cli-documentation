# VPN

The **vpn** command lets you manage VPNs to connect to HackTheBox machines.

## Download VPNs

The `-d` or `--download` flag **downloads all VPNs** assigned to the user.
The **VPN configuration files** will be downloaded to the following folder: `~/.local/htb-cli/`

```bash
htb-cli vpn --download
```

![Download](/assets/commands/vpn/download.png)

## List assigned VPNs

The VPNs assigned can be listed with the `--list` flag.

```bash
htb-cli vpn --list
```

![List](/assets/commands/vpn/list.png)


## Starting a VPN

A VPN can be started with the `--start` flag.
The **mode** must be specified with the `-m` flag from the following list:

* labs
* sp
* fortresses
* prolabs
* endgames
* competitive

```bash
htb-cli vpn -m labs --start
```

![Start](/assets/commands/vpn/start.png)

## Stop the VPN

We can also stop the active VPN with the `--stop` flag.

```bash
htb-cli vpn --stop
```

![Stop](/assets/commands/vpn/stop.png)