# rake fast

Fast rake autocompletion plugin for [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

## What?

This script caches the output for later usage and significantly speeds it up.

It generates a file .rake_tasks in parallel to the Rakefile. It also checks the file modification dates to see if it needs to regenerate the cache file.

This is entirely based on [this pull request by Ullrich Schäfer](https://github.com/robb/.dotfiles/pull/10/), which is inspired by [this Ruby on Rails trick from 2006](http://weblog.rubyonrails.org/2006/3/8/fast-rake-task-completion-for-zsh/).

Think about that. 2006.

## How to install

1. Clone this repository in oh-my-zsh plugins directory:

  ```bash
  cd ~/.oh-my-zsh/custom/plugins
  git clone git://https://github.com/KevinBongart/rake-fast.git
  ```

2. Add the plugin to your `.zshrc`:

  ```bash
  plugins=(foo bar rake-fast)
  ```

3. Source `~/.zshrc` to take changes into account:

  ```bash
  source ~/.zshrc
  ```

You'll also want to add `.rake_tasks` to your [global .git_ignore](https://help.github.com/articles/ignoring-files#global-gitignore)
