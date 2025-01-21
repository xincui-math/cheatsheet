# TMUX Cheatsheet

---

## Session Management

| Command                              | Description                                         |
|--------------------------------------|-----------------------------------------------------|
| `tmux`                               | Start a new session                                |
| `tmux new -s [name]`                 | Start a new session with a name                   |
| `tmux attach`                        | Reattach to the last session                      |
| `tmux attach -t [name]`              | Attach to a specific session                      |
| `tmux list-sessions` (`tmux ls`)     | List all sessions                                 |
| `tmux detach` (`Ctrl-b d`)           | Detach from the current session                   |
| `tmux kill-session -t [name]`        | Kill a specific session                           |
| `tmux kill-server`                   | Kill all tmux sessions                            |

---

## Window Management

| Command                              | Description                                         |
|--------------------------------------|-----------------------------------------------------|
| `Ctrl-b c`                           | Create a new window                                |
| `Ctrl-b ,`                           | Rename the current window                         |
| `Ctrl-b n`                           | Move to the next window                           |
| `Ctrl-b p`                           | Move to the previous window                       |
| `Ctrl-b w`                           | List windows and select one interactively         |
| `Ctrl-b &`                           | Close the current window                          |
| `tmux select-window -t [index]`      | Select a window by index                          |

---

## Pane Management

| Command                              | Description                                         |
|--------------------------------------|-----------------------------------------------------|
| `Ctrl-b %`                           | Split pane vertically                              |
| `Ctrl-b "`                           | Split pane horizontally                            |
| `Ctrl-b o`                           | Switch to the next pane                           |
| `Ctrl-b ;`                           | Toggle between the last two panes                 |
| `Ctrl-b q`                           | Show pane numbers                                  |
| `Ctrl-b x`                           | Close the current pane                            |
| `Ctrl-b z`                           | Toggle zoom for the current pane                  |
| `tmux select-pane -t [index]`        | Select a pane by index                            |
| `Ctrl-b {`                           | Swap pane with the previous one                   |
| `Ctrl-b }`                           | Swap pane with the next one                       |
| `Ctrl-b Space`                       | Cycle through pane layouts                        |

---

## Resizing Panes

| Command                              | Description                                         |
|--------------------------------------|-----------------------------------------------------|
| `Ctrl-b Ctrl-[arrow key]`            | Resize pane in the specified direction            |
| `tmux resize-pane -L`                | Resize pane to the left                           |
| `tmux resize-pane -R`                | Resize pane to the right                          |
| `tmux resize-pane -U`                | Resize pane upwards                               |
| `tmux resize-pane -D`                | Resize pane downwards                             |

---

## Copy Mode

| Command                              | Description                                         |
|--------------------------------------|-----------------------------------------------------|
| `Ctrl-b [`                           | Enter copy mode                                    |
| `Ctrl-b ]`                           | Paste copied text                                 |
| `q`                                  | Exit copy mode                                    |
| `Space`                              | Start text selection                              |
| `Enter`                              | Copy selected text                                |
| `Ctrl-b PageUp`                      | Scroll up in copy mode                            |
| `Ctrl-b PageDown`                    | Scroll down in copy mode                          |

---

## Session/Window Sharing

| Command                              | Description                                         |
|--------------------------------------|-----------------------------------------------------|
| `tmux new-session -t [session]`      | Create a new session linked to an existing one    |
| `tmux switch-client -t [session]`    | Switch to another session                        |
| `tmux move-window -s [src] -t [dst]` | Move a window between sessions                   |

---

## Customization

| Command                              | Description                                         |
|--------------------------------------|-----------------------------------------------------|
| `set-option -g prefix C-a`           | Change the prefix key to `Ctrl-a`                 |
| `unbind-key [key]`                   | Unbind a specific key                             |
| `bind-key [key] [command]`           | Bind a key to a specific command                  |

---

## Miscellaneous

| Command                              | Description                                         |
|--------------------------------------|-----------------------------------------------------|
| `Ctrl-b t`                           | Show current time                                 |
| `Ctrl-b ?`                           | List all key bindings                             |
| `tmux info`                          | Show information about the tmux server            |
| `Ctrl-b :`                           | Open command prompt in tmux                       |
| `Ctrl-b s`                           | List all sessions and windows                     |

---

## Scripting and Advanced Usage

| Command                              | Description                                         |
|--------------------------------------|-----------------------------------------------------|
| `tmux source-file [file]`            | Source configuration from a file                  |
| `tmux save-buffer [file]`            | Save buffer to a file                             |
| `tmux load-buffer [file]`            | Load buffer from a file                           |
| `tmux pipe-pane -o [command]`        | Pipe output of a pane to a shell command          |
| `tmux display-message [msg]`         | Display a custom message                          |
