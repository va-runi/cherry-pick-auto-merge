# cherry-pick-auto-merge
This is useful to reduce the time spent on merging the changes from master to a release branch. We dont need to wait for developers to cherry pick and create PR and wait for approvers to approve.
It cherry picks a commit from source branch and auto merge to a target branch

What does it do?
1) create a new branch in target branch(eg: release branch) and checkout
2) cherry pick a commit from source branch(eg: master)
3) create a PR to merge new branch into the target branch with cherry picked commit
4) auto merge the PR to target brach if it meets all requirements like successful build and sonar pass and no conflicts
