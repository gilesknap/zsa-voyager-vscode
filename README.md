# Some goals to keep up coding skills


## RSI avoidance
Learn zero glances at the keyboard.
Learn keyboard only in vscode.
- to this end I replaced the x-bows with a ZSA Voyager
    - https://www.zsa.io/voyager/
    - made some vscode keybindings for the Hyper thumb key as per this file
      - [keybindings.json](keybindings.json)
    - and this config
      - https://configure.zsa.io/voyager/layouts/pDAzE/latest/0
    - plus picked [monkeytype](https://monkeytype.com/) as a typing tutor
- idea 2: use a trackball with no switches instead of mouse, the navigation layer I
  made for the keyboard already has left hand mouse buttons plus everything else
  I imagine I need - will see how effective this is when the trackball arrives:
  - https://ploopy.co/nano-trackball/
  - terrible name but only product like it I could find

## vscode Keybindings on the Hyper Keys

See [keybindings.json](keybindings.json)

Note that there can be clashes with ctrl shift u for unicode input, and ctrl
shift e for emoji input. To disable run ```ibus-setup``` and change or remove
the keybindings that use ctrl shift u and ctrl shift e. Also on RedHat I
needed the following to make this work:

```bash
export GTK_IM_MODULE=ibus
export XMODIFIERS=@im=ibus
export QT_IM_MODULE=ibus
```

![vscode keybindings](vscode.svg)