# more common git commands
[[Manuale git]]

clone a remote project

	git clone <remote address>

keep track of modified file

	 git add <file>

commit changes

	git commit -m "comment message"

send a commit to remote repository
branch is the branch you want send to host, origin is the remote host you want update

	git push origin <branch> 
	
get updates from remote host
main is your branch you want update, origin is the remote host from you get new commits

	git pull origin main

to add an origin (origin is an arbitrary name)

	git remote add origin https://github.com/giuliofalco/......
