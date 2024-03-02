# gh-events

References:
- Main page: https://docs.github.com/en/actions/using-workflows
- Pull request: https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#pull_request
- Syntax on.push: https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#onpushbranchestagsbranches-ignoretags-ignore
- Filter pattern cheat sheet: https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#filter-pattern-cheat-sheet
- Skip workflow runs: https://docs.github.com/en/actions/managing-workflow-runs/skipping-workflow-runs


Items covered in the course are bellow: 

This course covers witch set of filters (event types) we can add for a workflow event listener 

![](gh-event.png?raw=true)

- Only collaborator are eligible to activate the workflow even it maches with the events and filters inserted
- If the person who opened the PR is not a collaborator the workflow will keep pending until the owner approve it.

![](collaborator.png?raw=true)

- For example:

![](approve.png?raw=true)

- If your commit will trigger any job and for exemple, your change is only a comment (not a code change) you can opt to skip it.
- in your commit you can pass some of the skip commands lited in the links above.
- Exemple git commit -m "added commnents [*skip ci*]"

- Summary:

![](summary.png?raw=true)