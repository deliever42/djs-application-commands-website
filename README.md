---
description: Welcome!
---

# Introduction

## What is This Module?

#### The purpose of this module is to use Discord's renewed application commands (permission v2) with discord.js. This module brings all the features of Discord's application commands. Good coding!

## Dependencies

```
discord.js >= 13.6.0
@discordjs/collection >= 0.6.0
@discordjs/rest >= 0.4.1
@sapphire/snowflake >= 3.2.2
```

## Installation

Node.js 16.9.0 or newer is required.

```
npm install djs-application-commands
```

## Example

```javascript
const { Client, Intents } = require('discord.js');
const client = new Client({
    intents: [Intents.FLAGS.GUILD_MESSAGES, Intents.FLAGS.GUILDS],
});

const {
    ApplicationCommandManager,
    ApplicationCommandBuilder,
} = require('djs-application-commands');

client.on('ready', async () => {
    client.applicationCommandManager = new ApplicationCommandManager(client);

    const commands = [
        new ApplicationCommandBuilder()
            .setName('ban')
            .setGlobal(false)
            .setPermissions(['BAN_MEMBERS'])
            .setDescription('Ban a member')
            .addUserOption(builder => {
                builder
                    .setName('user')
                    .setDescription('User to ban')
                    .setRequired(true);
            })
            .addStringOption(builder => {
                builder
                    .setName('reason')
                    .setDescription('Reason to ban')
                    .setRequired(false);
            })
            .addIntegerOption(builder => {
                builder
                    .setName('deleteMessageDays')
                    .setDescription('Number of days of messages to delete')
                    .setMaxValue(7)
                    .setMinValue(1)
                    .setRequired(false);
            }),
        new ApplicationCommandBuilder()
            .setName('ping')
            .setGlobal(true)
            .setDescription("Get the bot's ping"),
    ];

    const guildCommands = commands.filter(cmd => !cmd.global);


    //saving commands
    client.applicationCommandManager.set(commands);

    //saving commands on new guild
    client.on('guildCreate', guild => {
        client.applicationCommandManager.set(guildCommands, guild.id);
    });

    client.on('interactionCreate', async interaction => {
        if (interaction.isApplicationCommand()) {
            const cmd = client.applicationCommandManager.cache.get(interaction.commandName);
            if (!cmd) return;

            await interaction.deferReply({ ephemeral: true });

            switch (cmd.name) {
                case 'ping':
                    await interaction.followUp({
                        content: `Pong! :ping_pong: **${client.ws.ping}**ms`,
                    });
                    break;
                case 'ban':
                    const user = interaction.options.getUser('user');
                    const reason = interaction.options.getString('reason') ?? 'No Reason Provided.';
                    const deleteMessageDays = interaction.options.getInteger('deleteMessageDays');

                    interaction.guild.bans
                        .create(user.id, { reason, days: deleteMessageDays })
                        .then(async () => {
                            await interaction.followUp({
                                content: 'This user successfully banned.',
                            });
                        })
                        .catch(async () => {
                            await interaction.followUp({
                                content:
                                    "An error occurred while banning the member. The member's authority may be above my authority.",
                            });
                        });

                    break;
            }
        }
    });
});

client.login('your-token-goes-here');
```
