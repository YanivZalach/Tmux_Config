# My Awesome Tmux Configuration


Tmux is a terminal multiplexer that allows you to split your terminal into multiple panes and windows, enhancing your productivity by providing a seamless way to manage and organize your terminal sessions. It's like having multiple terminals within one, all in a single window.


What do we have here? My Tmux configuration file!🪄


Who can use it? Anyone can use it!📺

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

     - 🔄 `C-a r`: Reload your Tmux configuration.


     - 🪟 `C-a q`: Confirm and kill the current pane.
     - 🚪 `C-a X`: Confirm and kill the current window.
     - 🪟 `C-a Q`: Confirm and kill the entire session.


     - 🧲 `C-a s`: Detouch (quit and save) Tmux session.
     - 🪟 `C-a c`: Create a new Tmux window.
     - 🔃 `C-a C-o`: Rotate windows (circularly).


     - 📛 `C-a M`: Rename the current session.
     - 🖍️ `C-a m`: Rename the current window.


     - 🔀 `C-a t`: Move to the next window.
     - 🔀 `C-a T`: Move to the previous window.

 * Pane Management 🪟

     - 🔗`C-a S`: Synchronize panes.
     - 📊`C-a d`: Display pane numbers.


     - ➡️ `C-a x`: Split the current pane horizontally (x axis).
     - ⬇️ `C-a y`: Split the current pane vertically (y axis).
     - 📊`C-a C-y`: Use a horizontal layout.
     - 📊`C-a C-x`: Use a vertical layout.
     - ⏩`C-a Enter`: Switch to the next layout.


     - ⬅️ `M-Left`: Move to the pane on the left.
     - ➡️ `M-Right`: Move to the pane on the right.
     - ⬆️ `M-Up`: Move to the pane above.
     - ⬇️ `M-Down`: Move to the pane below.


     - ⬅️ `C-a h`: Move to the pane on the left.
     - ⬇️ `C-a j`: Move to the pane below.
     - ⬆️ `C-a k`: Move to the pane above.
     - ➡️ `C-a l`: Move to the pane on the right.
     - 🧩`C-a e`: Move to the previously active pane.


     - ➡️ `C-a H`: Resize the current pane leftwards.
     - ⬇️ `C-a J`: Resize the current pane downwards.
     - ⬆️ `C-a K`: Resize the current pane upwards.
     - ➡️ `C-a L`: Resize the current pane rightwards.

* Copy Mode 📋

     - 📋`C-a [`: Enter copy mode.
     - 📋`C-a ]`: Paste from the clipboard.


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
