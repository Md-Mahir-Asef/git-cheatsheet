# Git Cheatsheet
This is a cheat sheet for git commands and git workflows.

## Common Git Commands
### Branches
1. Create a new branch and checkout to that:
```bash
git checkout -b branch-name
```
2. Checkout to an existing branch:
```bash
git checkout branch-name
```
3. Delete a branch:
```bash
git branch -D branch-name
```
4. List only local branches:
```bash
git branch
```
5. List only remote branches:
```bash
git branch -r
```
6. List all branches (local + Remote):
```bash
git branch -a
```
7. Show branches with last commit info (more detailed):
```bash
git branch -vv
```

## Git Workflows
### Git Branch Workflow
1. Check out from the current branch and create a new branch. 
```bash
git checkout -b type/name
```
2. After finishing the work 
```bash
git add .
git commit -m "type: short description about the work you have done."
```
3. Push the branch to the remote so it is backed up.
```bash
git push -u origin type/name
```
4. Then open a PR (Pull Request) if you are done.
5. Merge to main according to team rules and permissions.
6. 
#### If you need to back out before the merge.
You can easily come back because your main is untouched.
```bash
git checkout main
```
You can again go to the main branch.
```bash
git checkout main
```
You can also delete the previous branch.
```bash
git branch -D type/name
```
