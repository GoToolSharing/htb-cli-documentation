# Introduction

This section describes each command available via **htb-cli**. In addition, this page explains the functionality of the **global flags** for each command.

## Batch (--batch)

This flag allows you to answer **"yes"** to any question that may be asked by htb-cli.

```bash
htb-cli info -c OOPArtDB --batch
```

![Batch](/assets/commands/globals/batch.png)

<!-- ## No Check (--no-check)

By default, with each command, a request is sent to **Github** to check if the tool is **up to date** or if a **new version is available**.

The `--no-check` flag allows you not to check if a new update is available. -->

## Proxy (--proxy)

The `--proxy` flag is used to route all htb-cli **traffic to a proxy** (e.g. BurpSuite).

```bash
htb-cli info --proxy http://127.0.0.1:8080
```

## Verbose (-v)

The **verbose flag** displays more information during program execution.
It has 2 levels:

* Level 1 displays **additional information**.
* Level 2 displays **debug information**.