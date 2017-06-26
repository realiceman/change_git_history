# Changing the Git history of your repository using a script

Open Terminal.

Create a fresh, bare clone of your repository:

git clone --bare https://github.com/user/repo.git
cd repo.git

Copy and paste the script, replacing the following variables based on the information you gathered.

Push the corrected history to GitHub:  
git push --force --tags origin 'refs/heads/*'


Clean up the temporary clone:
cd ..
rm -rf repo.git

