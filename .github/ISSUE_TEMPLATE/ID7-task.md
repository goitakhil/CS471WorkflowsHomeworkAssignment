---
name: '#7 Task'
about: 'Task that should be linked to user story #1'
title: 'Squash with Traceability to Task and PR in Commit Message Integration Strategy, without Any Commits in the Branch Referencing the Task'
labels: ''
assignees: ''

---

References user story #1

NOTE: the commits in the branch `task-7_squash_preferred_project_workflow` **DO NOT** reference task `#7`, and this is why this is the **preferred workflow** for the second half of Sprint 2 and Sprint 3 of the group project, and can be used for open-source or industry projects as well.

## TODO:
- [ ] Create a new PR having the **base** branch `master` and the **compare** branch `task-7_squash_preferred_project_workflow`
- [ ] Edit the description of the PR to reference this task
- [ ] Understand the commits and changes made to the PR
    - :thumbsup: notice that the commits in the branch **DO NOT** reference this task `#7`. This is intentional, as to not clutter this task with references of commits containing partial implementations (i.e., that do not contain the entire change in one commit), and which can be altered in subsequent commits in the same branch
- [ ] In the PR, use the `Squash and merge` option to integrate the changes into `master` and the commit message should be `Closes #6 (#<ID_PR>)`, and remove the extended description in the commit
- [ ] Use the GitHub interface to delete the branch of the PR after successfully integrating it into `master`

## Advantage of this workflow
:thumbsup: Any developer inspecting the commit in `master` can directly navigate
- to task `#6`, which will be referenced by only one "atomic" commit containing the final implementation of the task, and this commit can be [cherry-picked](https://git-scm.com/docs/git-cherry-pick) to other branches if needed, or
- to the PR (to see all the intermediate commits for the implementation, without any traceability to the task, and hence, without cluttering the task with references of partial commits)

Again, it is important to highlight that the commits in the branch **DO NOT** reference this task `#6`. Thus, developers can contribute to the branch without worrying about traceability for every intermediate step, and they can establish the traceability to the task and PR only once, during the integration.

