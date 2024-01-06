# Some ideas for making keyboards work harder for developers

## vscode Keybindings on the Hyper Keys

Hyper [key ctrl shift alt cmd] gives the ability to make keybindings that
don't clash with anything else. The point is not to try contort your fingers
to press all four keys at once, but to configure your keyboard to have a
single keypress mapped to the Hyper key.

Custom keyboards can be configured with a Hyper key. For standard keyboards
see below.

Here are some keybindings for vscode that
enable easy pane navigation and layout management.

WARNING: Although I'm from the UK, I use a US keyboard layout. UK keyboard
users will need to change the `\` to `[` for the layout to make sense. Other
layouts may need other changes.

One other point, if you have an
[ortholinear](https://www.daskeyboard.com/blog/what-is-an-ortholinear-keyboard/)
then they layout will be really tidy and look exactly like the diagram below.
If you don't then the keys will be offset a little. If you are thinking about
getting a new keyboard then I highly recommend ortholinear. You will have
a learning curve, but it is worth it.


See [keybindings.json](keybindings.json) for the vscode bindings to merge into
~/.config/Code/User/keybindings.json.

Note that the J-K-L and I keys effectively allow you to have
arrow keys for jumping around editor groups / sidebar / terminal panes.


![vscode keybindings](vscode.svg)

### Non custom keyboard owners

I believe that standard keyboard users could take advantage of these keybindings
by configuring their keyboard to have a Hyper key. This appears to say that
it can be done on linux:
https://gist.github.com/nat-418/135a62fb9f37cc87cd70af1ab72e276a


### Some minor niggles

Note that there can be clashes with ctrl shift u for unicode input, and ctrl
shift e for emoji input. It is odd because these seem to be ignoring the fact
that the meta and alt modifiers are also pressed. It looks like ``ibus`` is
to blame and has bugs.

To disable run ```ibus-setup```, go to the "emoji" pane and change or remove
the keybindings that use ctrl shift u and ctrl shift e. Also on RedHat I
needed the following in my bash profile to make this work:

```bash
export GTK_IM_MODULE=ibus
export XMODIFIERS=@im=ibus
export QT_IM_MODULE=ibus
```
