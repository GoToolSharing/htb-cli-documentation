# Submit

The **submit** command is used to **submit a flag**. Currently, the following submissions are supported :

* VIP machines
* VIP+ machines
* Free machines
* Release Arena machines
* Challenges

The `-d` or `--difficulty` flag must be used to indicate the **difficulty** of obtaining the flag.

## Active machine

If there is no `--machine` or `--challenge` flag, submission will be made on the **current active machine**.

```bash
htb-cli submit -d 3
```

![Active](/assets/commands/submit/active.png)

## Find a machine

A **machine name** can be specified to submit the flag for a specific machine. The `-m` or `--machine` option can be used for this.

```bash
htb-cli submit -m Sau -d 3
```

![Machine](/assets/commands/submit/machine.png)

## Challenge

To **submit a challenge** flag, you can specify its name with the `-c` flag.

```bash
htb-cli submit -c OOPArtDB -d 10
```

![Challenge](/assets/commands/submit/challenge.png)