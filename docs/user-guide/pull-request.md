# Pull Requests
## Best Practices
PR should be created after the first commit from the feature/ or fix/ branch. 

Include a descriptive title, summarizing the components included in the PR. 

The PR template included below, should be included for each PR. 

PRs may be created in draft or review mode. 

Drafts can only be edited by the individual who created them. 

For collaborative branches, review-mode PR’s may be used. 

Upon completion of the PR template and testing, a userd that is not the PR requestor should be assigned as a reviewer, that is not the PR requestor. 

After a review, address any concerns, updating the PR as needed. 

Complete the Code Review cycle until approval is achieved from the reviewer. 

Upon approval from the reviewer, push the branch into dev or main under the following conditions: 

Main: Any break-fixing patch updates 

Dev: All other updates 

Ensure the feature or fix branch has been deleted. 

## Tutorial
### Create the PR
1. Go to your Github page and select `Pull Request` > `New pull request`

2. Merge your `feature/update_contributions` branch into `dev`, then `create pull request`

3. Copy the template into your pull request
```
# Changes 

**This PR includes the following changes:** 

```list of changes, for example: 
- feat: Added processing of Ion-torrent Bams and ONT long reads 
- feat: Added Nanoplot as Quality metrics tool for ONT long reads 
- feat: Samtools ampliconclip is used as primary trimming tool for ONT-long reads. 
- fix: removed ivar trim which was erroring for ONT-long reads```

# Issues 
**This PR addresses the following issues:** 
```list of issues, for example: - fixes #17```

# Scope 
**Limitations:** 
```for example, only tested on HPC cluster Rosalind```

# Checklist 
The following points were addressed in this PR: 
- [ ] Description of the changes with justifications and issue links, where applicable 
- [ ] Updated docs related to these changes 
- [ ] Updated `CHANGE.md` with changes outlined above and a reference to the PR number.
```
4. Update the information above, including your previous issue.

NOTE: Notice that there are rules and CI available! All PR's should have a reviewer in real-work.

5. Merge pull request and confirm. Delete branch.
