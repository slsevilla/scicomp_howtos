# Feature Branch

## Best practices
Each repository must have the following two branches at any time, with additional branches created to address `features` or `fixes` 

- ‘main’ (titled ‘main’ or ‘master’) 

- ‘dev’ (titled ‘dev’ or ‘develop’)

New branches should adopt the style of `feature/<feature_name>` or `fix/<patch_description>`

A new, descriptive branch is created for each new feature or fix using `git checkout -b <branch name>` 

Branch source will vary depending on need (i.e.,IE main, dev, feature, or fix) 

Ideally, each would be linked to an issue, which would be included, such as: `feature/issue79_add_ivar_trim` or `fix/issue80_primer_error` 

Changes to feature/ and fix/ branches are merged into `dev` branch, following Pull Request (PR) SOP. 

Upon merging, feature/ or fix/ branch is deleted. 

## Tutorial

### Create the dev branch
1. Check what branches are available
```
git branch -a
```

2. Create a new branch called dev; verify the branch exists
```
git checkout -b dev
git branch -a
```

3. Push this new branch to your repo
```
git push origin dev
```

4. Go to your github page and refresh - you should see there is a new branch listed under the dropdown [main is listed as default]

### Create a feature branch
1. Return to your git terminal and ensure that you are on the dev branch
```
git branch -a
```

2. Create a feature branch based on the dev branch
```
git checkout -b feature/update_contributions
```

3. Edit the contributions page
```
vim docs/user-guide/contributions.md

git add docs/user-guide/contributions.md

git commit -m "docs: added contributions"

git push origin feature/update_contributions
```