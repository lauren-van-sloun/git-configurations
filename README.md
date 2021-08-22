# git-configurations
Holds my favorite git configurations so I can more quickly set up a new environment

## Set aliases

- To create/modify a single alias, use the command
    - `git config --global alias.cob 'checkout -b` or `git config --global alias.s status`
    
- To create/modify many at once, open your global git config file (can use the command `git config --global --edit`) and add:
  
  ```
  [alias]
	  last = log -1 HEAD
	  co = checkout
	  cob = checkout -b
	  s = status
	  cm = commit -m
	  alias = config --get-regexp ^alias\\.
	  a = add
	  aa = add .
	  b = branch
	  c = commit
	  com = checkout main
	  cod = checkout develop
	  bd = branch -D
	  pom = pull origin main
	  mm = merge main
	  sl = stash list
	  sa = stash apply
	  sp = stash pop
	  remote-commits = rev-list --all --remotes --pretty
	  md = merge develop
	  pod = pull origin develop
	  outta-here = reset --hard
  ```

## Set name and email
- `git config --global user.name 'Lauren Rutledge'`
- `git config --global user.email email@address.com`

## Generate a new SSH key to authenticate to GitHub
- https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key
