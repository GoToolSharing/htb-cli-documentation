# Submit

The **submit** command is used to **submit a flag**. Currently, the following submissions are supported :

* VIP machines
* VIP+ machines
* Free machines
* Release Arena machines
* Challenges
* Fortresses

## Achievements

When submitting a flag with the **submit command**, if the user has submitted both the user flag and the root flag, a link to the user's achievement will be displayed.

```bash
htb-cli submit -m Shoppy
```

![Achievement](/assets/commands/submit/achievement.png)

![Achievement2](/assets/commands/submit/achievement2.png)

## Release Arena

If no flag is submitted, then the machine in **release arena** will be chosen. The machine in **release arena** can also be searched via the `-m` or `--machine` flag.

```bash
htb-cli submit
```

![Machine](/assets/commands/submit/ra.png)

## Machine

A **machine name** can be specified to submit the flag for a specific machine. The `-m` or `--machine` option can be used for this.

```bash
htb-cli submit -m Sau
```

![Machine](/assets/commands/submit/machine.png)

## Challenge

To **submit a challenge** flag, you can specify its name with the `-c` or `--challenge` flag.

The `-d` or `--difficulty` flag must be used to indicate the **difficulty** of obtaining the flag.

```bash
htb-cli submit -c OOPArtDB -d 10
```

![Challenge](/assets/commands/submit/challenge.png)

## Fortress

To **submit a fortress** flag, you can specify its name with the `-f` or `--fortress` flag.
The exact name is not essential. A **fuzzy finder** will retrieve the fortress with the name closest to the search.

```bash
htb-cli submit -f text
```

![Fortress](/assets/commands/submit/fortress.png)

## Prolabs

To **submit a prolab** flag, you can specify its name with the `-p` or `--prolab` flag.
The exact name is not essential. A **fuzzy finder** will retrieve the prolab with the name closest to the search.

```bash
htb-cli submit --prolab Dante
```

![Prolab](/assets/commands/submit/prolab.png)