# dotfiles

<img width="3440" height="1440" alt="image" src="https://github.com/user-attachments/assets/78e57b79-9849-418d-8332-4e17682c207d" />

My minimalist Arch Linux configuration with the focus on productivity and usability, featuring:
- window manager: i3
- compositor: Picom
- bar: Polybar
- switcher: Rofi
- terminal emulator: Alacritty
- shell: Zsh

Key config aspects include:
- the Dvorak programmer keyboard layout (the only one I touch type on),
- crucial key combinations and shortcuts for 60% keyboard,
- left-handed trackball config,
- low contrast colorschemes - easy on the eyes,
- Picom for clean, minimal blur and shadow effects.
- vi-mode for basically everything to keep the hands on the keyboard


## Basic navigation levels

The navigation is designed to allow easy switching between the three main
levels as follows:

1. **Meta+Tab** cycles through workspaces
2. **Alt+Tab** cycles through windows in a workspace
3. **Ctrl+Tab** cycles through tabs in an application window

Some apps fit very nicely into this concept (e.g. Firefox) while others
required a significant amount of tweaking (see the tmux config 'hack' for
example).


### tmux

The leader shortcut has been remapped to Ctrl+S. The default Ctrl+B feels a
tiny bit clumsy to me but probably the main factor behind this decision was to
override the default Ctrl+S behaviour which pauses the output to the terminal
-- it's annoying when you press it by accident and suddendly you're trying to
figure out why nothing is working (which I have done countless times) and it's
a relic of a bygone era which on a modern machine only holds historical
significance without any practical use cases.


You'll see in the configuration that there's a 'Unicode hack' that in
combination with a custom Alacritty keybinding allows tmux to have Ctrl+Tab
(and Ctrl+Shift+Tab) to cycle through the windows as if they were tabs in any
other application.
