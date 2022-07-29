# discord-py-snippets
![Basic Usage](https://github.com/nerdguyahmad/discord-py-snippets/blob/main/assets/basic_snippet.gif)

VSCode extension providing useful and up-to-date snippets for discord.py 2.0.

**Features:**
- Consistent and easy to remember prefixes
- Carefully designed to suit common practices and uses
- Fully up-to-date with current version of discord.py

## Overview
This simple extension provides useful and commonly used snippets for discord.py.
The extension takes common practices of discord.py users into account to provide
snippets that fit most use cases.

## Snippets
All snippets are prefixed with `dpy.` for ease of usage.

### Starter Boilerplate

|     Prefix     |                                  Description                             |
|:--------------:|:------------------------------------------------------------------------:|
|    `dpy.bc`    |          Basic starter boilerplate based on `discord.Client` class.      |
|    `dpy.ac`    |       Advanced starter boilerplate based on `discord.Client` subclass.   |
|    `dpy.bb`    |          Basic starter boilerplate based on `commands.Bot` class.        |
|    `dpy.!`     |                           Shorthand for `dpy.bb`                         |
|    `dpy.ab`    |         Advanced starter boilerplate based on `commands.Bot` subclass.   |

### Basic

|     Prefix     |                                  Description                             |
|:--------------:|:------------------------------------------------------------------------:|
|    `dpy.ev`    |                 An event using the `Client.event` decorator.             |
|    `dpy.cmd`   |                 A command using the `Bot.command` decorator.             |
|    `dpy.lr`    |                 A listener using the `Bot.listen` decorator.             |

### Cogs and Extensions

|     Prefix     |                                  Description                             |
|:--------------:|:------------------------------------------------------------------------:|
|    `dpy.ext`   |                          Basic extension template.                       |
|    `dpy.cog`   | A cog template. Due to common practices, Also includes `setup` function  |
|    `dpy.ccmd`  |        A command for cogs using the `commands.command` decorator.        |
|    `dpy.clr`   |  A cog based listener using the `commands.Cog.listener` decorator.       |

### UI

|     Prefix     |                                  Description                             |
|:--------------:|:------------------------------------------------------------------------:|
|    `dpy.view`  |                          Basic `ui.View` template                        |
|    `dpy.btn`   |          Basic function based button using `ui.button` decorator.        |
|    `dpy.btnc`  |          Basic class based button by subclassing `ui.Button` class.      |

## Development experience
This extension is focused to bring an enhanced development experience. When generating a
snippet, you can simply type it's prefix and it's description, code and other information
will be shown by VSCode automatically.

You can press <kbd>Tab</kbd> to autocomplete the snippet. Each snippet is customizable
and you can press <kbd>Tab</kbd> to jump between common points of a snippet to modify
it according to your need.

![Developer Experience](https://github.com/nerdguyahmad/discord-py-snippets/blob/main/assets/developer_experience.gif)

## Contributing
This extension is powered by contributions! If you want to add a snippet, improve a current
snippet or suggest a snippet, feel free to read our [Contribution Guidelines](https://github.com/nerdguyahmad/discord-py-snippets/blob/main/CONTRIBUTING.MD)
