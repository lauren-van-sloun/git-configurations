# git-configurations
Holds my favorite git configurations so I can more quickly set up a new environment

## Set default text editor to Notepad++
- `git config --global core.editor "'C:/Program Files (x86)/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"`

## Set aliases

- To create/modify a single alias, use the command
    - `git config --global alias.cob 'checkout -b` or `git config --global alias.s status`
    
- To create/modify many at once, open your global git config file (can use the command `git config --global --edit`) and add:
  
  ```
  [alias]
      a = add
      aa = add .
      alias = config --get-regexp ^alias\\.
      b = branch
      bd = branch -D
      c = commit
      cm = commit -m
      co = checkout
      cob = checkout -b
      cod = checkout develop
      com = checkout main
      last = log -1 HEAD
      md = merge develop
      mm = merge main
      outta-here = reset --hard
      pod = pull origin develop
      pom = pull origin main
      remote-commits = rev-list --all --remotes --pretty
      s = status
      sa = stash apply
      sl = stash list
      sp = stash pop
  ```

## Set name and email
- `git config --global user.name 'Lauren Van Sloun'`
- `git config --global user.email email@address.com`

## Generate a new SSH key to authenticate to GitHub
- https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key
