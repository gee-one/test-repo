# test-repo

this is a repo for testing

# push commits to existing repo 

git push -u origin master


# create new repo from command line

echo "# test-repo" >> README.md

git init

git add README.md

git commit -m "first commit"

git remote add origin git@github.com:gee-one/<repo_name_goes_here>.git

git push -u origin master


# push existing repo from command line

git remote add origin git@github.com:gee-one/<repo_name_goes_here>.git

git push -u origin master


# set push to use ssh instead of https

git remote get-url --all origin

git remote get-url --push origin

git remote set-url  origin git@github.com:gee-one/<repo_name_goes_here>.git

# use gpg to sign commits
be sure to update .bashrc and don't forget the password
git commit -S -a {-m your commit message}
