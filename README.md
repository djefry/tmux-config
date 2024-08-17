# General
This is my tmux (terminal-multiplexer) configuration that I use along with vim or neovim.
We use tpm (tmux-plugin-manager) to install the plugin. In this configuration we can also use vim keybinding to move between tmux window when opening neovim.
We use tmux resurrect and tmux-continuum to restore the session and save the session every period of time, so when we start our machint the session is ready.

# How to Use
1. Install tmux plugin manager [tpm](https://github.com/tmux-plugins/tpm)
    By running this command `git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm`
2. Copy this config file to your home directory
3. Open tmux by executing `tmux`
4. Install the plugin by pressing `<prefix> + I (capital i, as in Install) to fetch the plugin.
5. In this configuration the previx is Ctrl + A, so after pressing Ctrl + A then press I
6. Your tmux is ready to use.
7. To create new session `tmux new -s your_session_name`
8. To attacth to previous session use command `tmux attach -t your_session_name`

# Favorite Shortcut
1. `<previx> + s` - save tmux session.
2. `<prefix> + w` - list all available session along with it's panes
3. `<prefix> + c` - create new panes in session
4. `<prefix> + ,` - rename active panes
5. `<prefix> + d` - detach the tmux session without exit the session
6. `<prefix> + |` - open new window by spliting current panes vertically
7. `<prefix> + -` - open new window by spliting current panes horizontally
8. `<Ctrl + h or j or k or l` - move between window in tmux panes using vim-motions
9. `<prefix> + :setw synchronize-panes` - sync all window in a panes or accepting same input in a time (everyting you type will shows and can be executed in all window) (this absolutely crazy!)
    To dissable it execute same command.
11. `<prefix> + number` - move to specifi panes using index (this only work for panes index under 10)
