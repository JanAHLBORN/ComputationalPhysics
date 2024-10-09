#---------------------------------------------#
# Definitions of most important technical terms
#---------------------------------------------#
* add: The git add command records all updates/changes you did and tells git to include them in the next   commit. 
* commit: snapshot of all changes made in a session (git saves the state of the project at this point).
* branch: List of changes you performed in some files. 
* push: Pushing is how you transfer commits from your local repository to a remote repo.
* merge request: This is a proposal to incorporate changes from a source branch. Developers can now check the changes and if they are allright the changes can be merged = incorporated in the project.


#-----------------#
# Conventions used
#-----------------#
We use the convention that all branches are created from the main branch on and get merge to it again. The branch names can be chosen arbitrarily. Any merge request needs to be approved by only one of us in order to be allowed to merge.



#------------------------------------#
# How to add, commit and push changes
#------------------------------------#
# First, always update your version of the project using pull
git pull
# Then, we create a branch and move to that branch using checkout
git checkout -b branch-xyz
# Make changes to your files
# Then add all changes
git add .
# Create a snapshot and add a commit message
git commit -m "Message that describes the changes"
# Eventually, push the branch (if it is the first push you might need to use "git push origin branch-xyz")
git push branch-xyz
# At this point on the website we get a notification for a merge request
# If the branch is merged it gets closed automatically