# Sherlocks

The **sherlocks** command lets you interact with HackTheBox's **blue team** mode. If no argument is given, you'll get information on **active, retired and soon-to-be-released** sherlocks.

```bash
htb-cli sherlocks
```

![Sherlocks](/assets/commands/sherlocks/sherlocks.png)

## Search & Download

You can add the `-s` argument to **search for a sherlock** with its name or part of its name, and the **fuzzy finder** will do the rest ! Another optional argument is `--download` or `-d`, which allows you to **download the resource** associated with the sherlock.

```bash
htb-cli sherlocks -s Meer --download /tmp/resources.zip
```

![Download](/assets/commands/sherlocks/download.png)

![File](/assets/commands/sherlocks/file.png)

## Submit solutions

To **submit** the answers for each task, you can add the `-t` or `--task` flag followed by the **task number**.

![Submit](/assets/commands/sherlocks/submit.png)

## Hint

Finally, the `--hint` flag can be added to provide a **hint**. If available, it will be displayed **above the masked flag** when a task is selected.