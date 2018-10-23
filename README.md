This is a proof of concept!

With this scripts you can prepare a shell demo session while still remaining flexible.

# Install

Drop the files in $HOME/bin.

# How it works

tmux-demo-start saves two environment variables in the tmux session it is
executed in:


    tmux set-environment TMUX_DEMO_SCRIPT "${TMUX_DEMO_SCRIPT}" # a text file
    tmux set-environment TMUX_DEMO_LINE 1 # the current line number

Also it binds CTRL-PageUp and CTRL-PageDown to execute tmux-demo-next or
tmux-demo-previous.

tmux-demo-next then prints the current line and increments the environment
variable TMUX_DEMO_LINE.
