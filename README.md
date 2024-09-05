# git-merge-test

>Use this repo to test Git funtionalities such as merge conflicts, squashes etc.

- `new-feature` branch I want to rebase into `main` but not have it leave another branch left over on the git history.
  - Adding in another comment to test.
  - And another commit
  - Used `git rebase -i HEAD~3` and then `f` to squash the commits and use the previous comments instead of `s` flag that you can then choose what comments to use.
  - Check the logs `git log --oneline`
  - Push to main with `git push origin <feature-branch> --force-with-lease`
  - Following these commands the branch was how I expected leaving no trace of the feature branch and keeping the "trunk" linear.

- If you do not delete the branch after rebasing, and then push to it again, you end up with a `merge conflict`?
- I think you have to get onto the "loose" branch that is hanging around, and rebase it into a previous commit.

- attempting to create
