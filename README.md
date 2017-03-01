# tmux Config

![](http://recordit.co/OxtY4mnBW7.gif)

## Steps

- Install `tmux`

- `gem install tmuxinator`

- Clone this repo & run below commands

- ```shell
  ln -s ~/path/to/dot/.tmux.conf ~/.tmux.conf
  ln -s ~/path/to/dot/my_dev.yml ~/.tmuxinator/my_dev.yml
  tmux source-file ~/.tmux.conf
  ```
- `.tmux.conf` needs to be loaded only once to rebind the settings

- To start `my_dev` tmux config - `tmuxinator start my_dev -n my_dev`

#### Notes

- Usual tmux keybinding has been modified to `Cntl-a` from `Cntl-b` (Because `a` is closer to Cntl than `b`)

- tmuxinator needs an editor flag to set in exports (default will be vim).
  If you wish to change, add the below line to `~/.zshrc`

  `export EDITOR="code"`

