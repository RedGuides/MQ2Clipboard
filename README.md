# MQ2Clipboard

I got sick of copying locs so I made this. Adds a single command, /clip -- alynel


## Commands

`/clip <text>` copies text to your clipboard  
`/clip <command>` runs a command and copies any chat output  
`/clip start`, followed by `/clip stop`, will copy any chat output that occurs between the two commands. This copies everything, MQ2 output and normal chat stuff  
`/clip command` will copy the last command you typed  

If you prefix anything with append, e.g. `/clip append <text>`, then it will append to the last thing it copied rather than overwriting it

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
