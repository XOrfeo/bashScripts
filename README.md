# bashScripts

This repository contains the bash scripts that I made to slow down insanity and fix minor inconveniences I encountered along the way.

## autoKBL

autoKBL is a script that [auto]matically sets the [k]ey[b]oard [l]ayout of a preconfigured set of keyboard devices if they are connected to your pc.
It looks for a file in your .config directory called autoKBL.list. This is a file you need to make yourself containing a layout and keyboard device name (in that order) separated by an unbroken pipe character '|' e.g.

```
gb|Logitech G513 RGB MECHANICAL GAMING KEYBOARD
```

If you are unsure of the correct device name, plug it in an run the command:

```bash
xinput -list
```

And you will find the name.

The script will output everything to a logfile that it will create in a .temp directory. It will also confirm any device layout changes to the user via the terminal it was run from.
