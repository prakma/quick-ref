# Quick reference for usually forgotten commands for Git

### Setup Git profile particular to a Git repo
git config user.email "mprakash@blah.com"

git config user.name "Manoj Prakash"

Run the above commands by going to the git repo folder

### Setup global git profile
git config --global user.email "you@example.com"

git config --global user.name "Your Name"

### To put existing code in a newly created github repo
1. Create a github repo
2. Clone into a temp directory
3. Move the .git file from the temp directory into the root directory of existing code
