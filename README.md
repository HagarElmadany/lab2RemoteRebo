 How remove branch Locally and Remotely?

 => to remove a local branch :
 1-switch to main branch :
 git checkout main
 2- delete local branch
 git branch -d branch_name

 => to remove a remote branch :
 git push origin --delete branch_name


********************************
Annotated tags vs Lightweight Tags

Annotated Tags: Store detailed information (name, email, date, message) and are used for important milestones or releases.
- Used for marking releases.
- To create an annotated tag:
git tag -a v2.0 -m “version 2.0”


Lightweight Tags: Simply point to a commit without extra metadata and are typically used for temporary or non-significant markers.
- Used for quick references or temporary markers.
- To create a lightweight tag"
git tag v1.0

****************************************
When to Use Rebase ?
 Rebase can be used to ensure that any other branch is up to date with the latest changes from the main branch.

 example when create main branch with 3 commit then create dev branch  then make new commit in main brach ,the dev branch canot see the fourth commit to make it see the last commit in main branch we use rebase

 -  git checkout dev
 -  git rebase main

 ************************
  How to List Tags ?

  To list all the tags in your repository, use the following command:
    - git tag
    - 