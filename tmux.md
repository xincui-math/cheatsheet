# TMUX Cheatsheet (Compact)

| **Session Management**      | **Window Management**   | **Pane Management**      |
|------------------------------|--------------------------|---------------------------|
| `tmux` Start session         | `Ctrl-b c` New window   | `Ctrl-b %` Split vertical |
| `tmux new -s [name]`         | `Ctrl-b ,` Rename       | `Ctrl-b "` Split horizontal |
| `tmux attach` Attach session | `Ctrl-b n` Next window  | `Ctrl-b o` Switch pane    |
| `tmux ls` List sessions      | `Ctrl-b p` Previous win | `Ctrl-b q` Show pane nums |
| `Ctrl-b d` Detach            | `Ctrl-b w` List windows | `Ctrl-b x` Close pane     |
| `tmux kill-session -t [n]`   | `Ctrl-b &` Kill window  | `Ctrl-b ;` Last pane      |

| **Copy Mode**               | **Resizing Panes**       | **Customization**         |
|------------------------------|--------------------------|---------------------------|
| `Ctrl-b [` Enter copy mode   | `Ctrl-b Ctrl-[arrow]`   | `set-option -g prefix X`  |
| `Ctrl-b ]` Paste buffer      | `tmux resize-pane -L`   | `unbind-key X` Remove key |
| `Space` Select text          | `tmux resize-pane -R`   | `bind-key X cmd` Bind key |
| `Enter` Copy selected text   | `tmux resize-pane -U`   | `source-file [file]` Load |
| `q` Exit copy mode           | `tmux resize-pane -D`   |                           |

| **Miscellaneous**           | **Advanced**             |                           |
|------------------------------|--------------------------|---------------------------|
| `Ctrl-b t` Time display      | `tmux save-buffer [f]`   |                           |
| `Ctrl-b ?` Key bindings      | `tmux load-buffer [f]`   |                           |
| `tmux info` Show details     | `tmux pipe-pane -o cmd`  |                           |
| `Ctrl-b :` Command prompt    | `tmux display-message`   |                           |
