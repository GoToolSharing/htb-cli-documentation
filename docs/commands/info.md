# Info

The **info** command will retrieve information from the **active machine** (if any) and display it. If no argument is supplied, the logged-in user's information will be displayed.

```bash
htb-cli info
```

![Info](/assets/commands/info/info.png)

## Player search

htb-cli allows you to retrieve information from **another player** via the `-u` flag, which will specify the desired **username**.

```bash
htb-cli info -u 22sh
```

![User Info](/assets/commands/info/user.png)

## Machine search

Information about a **machine** can also be retrieved with the `-m` flag followed by the **machine name**.

```bash
htb-cli info -m Bizness
```

![Machine](/assets/commands/info/machine.png)

## Challenge search

Information about a **challenge** can also be displayed with the `-c` flag followed by the **challenge name**.

```bash
htb-cli info -c OOPArtDB
```

![Challenge](/assets/commands/info/challenge.png)

## Combining search

Options can be **combined** to obtain user, machine and challenge information all at once, without having to re-run the command 3 times.

```bash
htb-cli info -c OOPArtDB -m Inject -u 22sh
```

![Combine](/assets/commands/info/combine.png)