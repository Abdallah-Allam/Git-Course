# Git_Course
pull Request =>is a feature in Git and GitHub that allows users to propose changes to a repository hosted on GitHub. It is a way to notify the repository owner or team that you have made changes to their code and that you would like them to review and potentially merge your changes into their repository.



## Command lines
git clone
git status
git add
git commit -m "message"
git pull origin main
git config => ! Important !
	git config -l, --list => list the configuration(not all of it)
	git config -l, --list --show-origin => display from where the configurations are
	git help config => list all the configurations
	git config --global user.name(example) => display the value of user.name
	git config --global user.name "a@gmail.com"(example) => set the value of user.name 
	git config --global user.name "" => empty the value of user.name
	git config --global --unset user.name => delete the user.name from configurations
	git config --global --edit => go to the editor and there you can edit the configurations from the editor

ssh-keygen -t rsa(Type Of Algorithm) -b(Bits) 4096 -C "email" => generat public key
	ssh -T git@github.com => test the public key on github after you added it

git init => Create an empty Git repository or reinitialize an existing one
	git add file_name => add the file to the staging area
	git commit -m "first commit" => commit it to the local repo
	git branch -m main => rename the branch(master) to main
	git remote add origin git@github.com:user-name/repo-name => add the your repo to the remote repo
	git push -u origin main => pull(-u) then push the files to the remote repo
	
git config --global alias.shortcut "command" => do shortcut with alias to any comman you want in 

git branch => display the branchs you have
	git branch name_of_branch => generate new branch with any name you want
	git checkout => switch the branchs
	git checkout name_of_branch => switch to "name_of_branch"
	git checkout -b new_branch => generate new branch and switch to it
	git branch -d name_of_branch => delete the branch but if the branch has new edits then the command does not delete it
	git branch -D name_of_branch => the command force the delete of the branch even if it has edits
	git branch -m new_name => rename the branch

git stash => stash your files in stashed place you can have it anytime you want
	git stash list => list the stashed file	
	git stash save "message" => save the file in stashed place with the message
	git stash pop => pull the stashed files from the stashed place and delete the stashed place, if there are multiple stashs it pulls the last stash you do
	git stash apply => pull the files from stashed place and keep the stashed place
	git stash pop (id)stash@{1} => pull the files from specific stash with its id and delete the stashed place
	git stash apply (id)stash@{1} => pull the files from specific stash with its id and keep the sptashed place
	git stash drop => delete the last stash you do
	git stash drop (id)stash@{2} => delete the stash with its id
	git stash show => display the content of the last stash you do
	git stash show (id)stash@{0} => display the content of the stash with its id
	git stash clear => clear all the stash you do
	

