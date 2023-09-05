# My Awesome Tmux Configuration

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

<p align="center">
   <img width="350" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e4/Tmux_logo.svg/800px-Tmux_logo.svg.png" alt="Tmux Logo">
</p>



Tmux is a terminal multiplexer that allows you to split your terminal into multiple panes and windows, enhancing your productivity by providing a seamless way to manage and organize your terminal sessions. It's like having multiple terminals within one, all in a single window.


What do we have here? My Tmux configuration file!🪄


Who can use it? Anyone can use it!📺

![tmux](https://github.com/YanivZalach/Tmux_Config/assets/131461377/acd4d292-4b95-4ded-9dad-31d2967c8f77)


## Requirements 📋

Before using this Tmux configuration, make sure you have the following installed on your system:

 * **Tmux**: Ensure Tmux is installed on your system.
  
 * **Terminal Emulator**: Use a compatible terminal emulator-you have probably one installed (e.g.,Kitty, Alacritty, GNOME Terminal).
  
 * `reattach-to-user-namespace`: Required for clipboard support on MacOS (installable via Homebrew).


## Installation 📦

 1. Install the programs listed above using your package manager or download them from their respective websites.
 
 2. Copy the config file:
     **Linux & MacOS & WSL:**
     Copy and paste the following command into the terminal and press 'enter':
     ```bash
     git clone https://github.com/YanivZalach/Tmux_Config.git ~/.Tmux_Config
     mv ~/.Tmux_Config/.tmux.conf ~/.
     
     ```
     
 3. **We are Done!**


## Usage, Features, and Special Key Bindings 🚀🪙

 **Get ready to supercharge your Tmux experience**


 **Features 🎉**
 * 🖱️ Mouse Support: Enjoy using the mouse in Tmux with your preferred terminal emulator.
 * ⏱️ Status Bar: Information-rich status bar displayed at the top.
 * 🔄 Automatic Renumbering: Windows are automatically renumbered to fill gaps.
 * 🔁 Immediate Window Switching: Quickly change windows using arrow keys.
 * 🌈 256 Colors: Supports 256-color terminals for a colorful experience.
     
 
**Key Bindings**

 * Prefix Key 🌟

     - 🎯 `C-a` , `C-z`: Your starting point. This is the prefix key. All Tmux commands begin with this key followed by another keybinding.

 * General Commands 🛠️

     - 🧲 `<Prefix> s`: Detouch (quit and save) Tmux session.
     - M  `<Prefix> :`: Command Prompt
     - 🔄 `<Prefix> r`: Reload your Tmux configuration.


     - 🪟 `<Prefix> q`: Confirm and kill the current pane.
     - 🚪 `<Prefix> X`: Confirm and kill the current window.
     - 🪟 `<Prefix> Q`: Confirm and kill the entire session.

     - 📋 `<Prefix> C-l`: Clearing the terminal window

 * Session Management 🪟

     - 📊`<Prefix> C-s`: Session Tree
     - 📛 `<Prefix> M`: Rename the current session.

 * Window Management 🪟

     - 🪟 `<Prefix> c`: Create a new Tmux window.
     - 🖍️ `<Prefix> m`: Rename the current window.

     - ⬅️ `S-Left`: Move to the Left window.
     - ➡️ `S-Right`: Move to the Right window.

     - 🔀 `C-S-Left`: Move window to the Left.
     - 🔀 `C-S-Right`: Move window to the Right .

     - 🔄 `<Prefix> t`: Move to the next window.
     - 🔄 `<Prefix> T`: Move to the previous window.
     - 🔃 `<Prefix> C-o`: Rotate windows (circularly).


 * Pane Management 🪟

     - 🔗`<Prefix> S`: Synchronize panes.
     - 📊`<Prefix> d`: Display pane numbers.


     - ➡️ `<Prefix> x`: Split the current pane horizontally (x axis).
     - ⬇️ `<Prefix> y`: Split the current pane vertically (y axis).
     - 📊`<Prefix> C-y`: Use a horizontal layout.
     - 📊`<Prefix> C-x`: Use a vertical layout.
     - ⏩`<Prefix> Enter`: Switch to the next layout.


     - ⬅️ `M-Left`: Move to the pane on the left.
     - ➡️ `M-Right`: Move to the pane on the right.
     - ⬆️ `M-Up`: Move to the pane above.
     - ⬇️ `M-Down`: Move to the pane below.


     - ⬅️ `<Prefix> h`: Move to the pane on the left.
     - ⬇️ `<Prefix> j`: Move to the pane below.
     - ⬆️ `<Prefix> k`: Move to the pane above.
     - ➡️ `<Prefix> l`: Move to the pane on the right.
     - 🧩`<Prefix> e`: Move to the previously active pane.


     - ➡️ `<Prefix> H`: Resize the current pane leftwards.
     - ⬇️ `<Prefix> J`: Resize the current pane downwards.
     - ⬆️ `<Prefix> K`: Resize the current pane upwards.
     - ➡️ `<Prefix> L`: Resize the current pane rightwards.

* Copy Mode 📋

     - 📋`<Prefix> [`: Enter copy mode.
     - 📋`<Prefix> ]`: Paste from the clipboard.


     - ✂️ `v:` Start selection (while in copy mode).
     - 📋`y:` Copy selected text to the system clipboard (in MacOS requires reattach-to-user-namespace).

## Troubleshooting 🔧

The installation is not working:

- Make sure you have Git installed on your computer.
  Open the terminal and run the following command:

  ```bash
  git --version
  ```

  If Git is installed, you will see the installed version. If not, you need to install it using your package manager.
  Then retry the Installation.
  
- Check if a file/directory already exists
  
  Check if the `~/.Tmux_Config` or `~/.tmux.conf` already exists.
  Open the terminal and run the following command to check if they exists:

  - To check if the `~/.tmux.conf` directory exists, run:

      ```bash
      cat ~/.tmux.conf
      ```

      Is found, run:

      ```bash
      mv ~/.tmux.conf ~/.tmux.conf_b
      ```

  - To check if the `~/.Tmux_config` directory exists, run:

      ```bash
      ls ~/.Tmux_Config
      ```

      Is found, run:

      ```bash
      mv ~/.Tmux_Config ~/.Tmux_Config_b
      ```
  Then retry the Installation.


## Acknowledgments 🙏

A special thanks to the Tmux community for their support.

### Happy Tmuxing! 🎉
