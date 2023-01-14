# learn-git
Learning git concepts and interview preparation


Git user and email setup :
System:
 /etc/gitconfig	

Global :
~/.gitconfig

Local ::
.git/config

Add below lines :
[user]
	email = rajendran.scm@gmail.com
	name = rajendra

Commands:
git config pull.rebase false  # merge
git config pull.rebase true   # rebase
git config pull.ff only       # fast-forward only

hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per


Push errors:
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

Git revert/reset :: 
Q: How to go back to particular commit of a file?
Git revert : but it makes another commit

Q: Reset to original state of git workspace?
 git reset --hard HEAD~1