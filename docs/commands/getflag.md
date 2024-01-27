# Getflag

The **getflag** command will make an **SSH connection** to a remote server and try to locate the **user.txt** file in the **home directories**. If the file is found, the flag is submitted directly via the HackTheBox API.

The `-u` / `--username` option is used to specify the **username**.

The `-p` / `--password` option specifies the **password**.

The `--host` option specifies the **hostname**.

The `-P` / `--port` option specifies the **SSH port** (Default: 22).

```bash
htb-cli getflag -u jaeger -p 'Sh0ppyBest@pp!' --host 10.10.11.180 -P 22 --batch
```

![Getflag](/assets/commands/getflag/demo.png)