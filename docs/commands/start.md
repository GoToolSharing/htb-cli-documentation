# Start

## Machine search

The **start** command starts an instance for a machine. The **machine name** must be specified using the `-m` or `--machine` argument. Once started, its **IP address** is displayed.

```bash
htb-cli start -m Visual
```

![Search](/assets/commands/start/search.png)

## Start the release arena machine

If **no flag** is submitted, htb-cli starts the machine in **release arena**.

```bash
htb-cli start
```

![Release Arena](/assets/commands/start/ra.png)

**Note:** The **release arena** machine can also be started by specifying its name with the `-m` flag.