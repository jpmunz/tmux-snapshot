Used this ruby script as a starting point:
https://github.com/geebee/tmux-persistence

Usage:
tmux-snapshot save
tmux-snapshot restore my-session

Working directories and last executed commands are remembered, history is not preserved. Googled around and didn't really find an existing solution that did this the way I wanted.

Common use-case is to have a crontab entry to continually save open sessions so that they can be restored after a reboot:

*   *   *   *   *   tmux-snapshot save
