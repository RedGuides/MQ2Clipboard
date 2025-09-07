---
tags:
  - command
---

# /clip

## Syntax

<!--cmd-syntax-start-->
```eqcommand
/clip [option] [</command|text>]
```
<!--cmd-syntax-end-->

## Description

<!--cmd-desc-start-->
Copies command output or text to your computer's clipboard
<!--cmd-desc-end-->

## Options

| Option | Description |
|--------|-------------|
| `<text>` | copies text to your clipboard |
| `</command>` | runs a command and copies any chat output |
| `append <text or command>` | Adds to the last thing on the clipboard, rather than overwrite. Can be a /command or text. |
| `start|stop` | "/clip **start**" will copy every line, both MQ and EQ output, until "/clip **stop**" is entered. |
| `command` | will copy the last command you typed |

## Examples

| If I type these commands... | Then paste here after the last command...                                    |
| :-------------------------- | :--------------------------------------------------------------------------- |
| `/clip hello world`         | hello world                                                                  |
| `/clip /loc`                | Your Location is 82.13, -296.06, -23.67, and are heading north by northwest. |
| `/clip command`             | /clip /loc                                                                   |
| `/clip start`               |                                                                              |
| `/echo test`                |                                                                              |
| `/echo test 123`            |                                                                              |
| `/clip stop`                | [MQ2] test                                                                   |
|                             | [MQ2] test 123                                                               |
| `/clip stuff`               | stuff                                                                        |
| `/clip append more stuff`   | stuff                                                                        |
|                             | more stuff                                                                   |
| `/clip append /loc`         | stuff                                                                        |
|                             | more stuff                                                                   |
|                             | Your Location is 82.13, -296.06, -23.67, and are heading north by northwest. |
| `/clip append command`      | stuff                                                                        |
|                             | more stuff                                                                   |
|                             | Your Location is 82.13, -296.06, -23.67, and are heading north by northwest. |
|                             | /clip append /loc                                                            |
