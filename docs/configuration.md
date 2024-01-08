# Configuration

## API token

In order to use `htb-cli`, you need to generate a **HackTheBox application token**. This token can be generated via your account configuration page: <a href="https://app.hackthebox.com/profile/settings" target="_blank">https://app.hackthebox.com/profile/settings</a>, then by clicking on **Create App Token**.

![Settings page](/assets/configuration/token.png)

You need to enter a **name** for the API token and an **expiry date**. In the following example, the name is **htbcli** and the expiry date is set to the maximum, i.e. **1 year**.

![New token](/assets/configuration/token-create.png)

The value of the token will be displayed only when it is created. Don't forget to **copy it**, otherwise you'll have to regenerate it.

![Token value](/assets/configuration/token-value.png)

This API token must be set in the `HTB_TOKEN` environment variable. You can add it directly to your **bashrc / zshrc** to make it permanent.

```bash
echo "export HTB_TOKEN=eyJ..."|tee -a ~/.zshrc
```

The shell must be refreshed for the changes to take effect. You can use the `source` command to reload the contents of the **bashrc / zshrc** file. Otherwise, when a new terminal is opened, the shell will be updated.

```bash
source ~/.zshrc
```

## Configuration file

A default configuration file is created the first time the tool is running at the following path : $HOME/.local/htb-cli/default.conf.
This is a Key / Value configuration file.

### Discord webhooks
The `Discord key` links `htb-cli` with discord webhooks.
First of all, to create a **webhook discord**, click on the **settings** button from a text channel.

![Webhook](/assets/configuration/webhook.png)

Next, click on the **Integrations** tab, then **Create a webhook**.

![New Webhook](/assets/configuration/new-webhook.png)

Copy the URL of the webhook and you can also change the bot's name.

![Webhook Copy](/assets/configuration/webhook-copy.png)

The link to the webhook must be added to the `htb-cli` configuration file (**~/.local/htb-cli/default.conf**) as shown in the example below.

```bash
Discord = https://discord.com/api/webhooks/*************/****************************
```

Now, for each `htb-cli` command, a message will be sent via the discord webhook.

![Discord](/assets/configuration/discord.png)

## Sanity check

The following command can be used to check that the installation has been carried out correctly.

```bash
htb-cli info --batch
```

![Profile](/assets/configuration/profile.png)
