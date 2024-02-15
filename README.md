# git
Cheatsheet for Git / Github

## Git
List your existing remotes in order to get the name of the remote you want to change.
```console
$ git remote -v
> origin  https://github.com/OWNER/REPOSITORY.git (fetch)
> origin  https://github.com/OWNER/REPOSITORY.git (push)
```

Change your remote's URL from HTTPS to SSH with the git remote set-url command.
```console
git remote set-url origin git@github.com:OWNER/REPOSITORY.git
```

Verify that the remote URL has changed.
```console
$ git remote -v
# Verify new remote URL
> origin  git@github.com:OWNER/REPOSITORY.git (fetch)
> origin  git@github.com:OWNER/REPOSITORY.git (push)
```

## Github
### SSH key 
Online documentation: [https://docs.github.com/en/authentication/connecting-to-github-with-ssh](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)
  - create a ssh key and add it to ssh-agent
  - add the new key to the github acount.
  
if `git push` requires username and password despite ssh: Switching remote URLs from HTTPS to SSH: see [Github documentation](https://docs.github.com/fr/get-started/getting-started-with-git/managing-remote-repositories#switching-remote-urls-from-https-to-ssh).