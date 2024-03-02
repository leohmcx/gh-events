# gh-events

References:
- Main page: https://docs.github.com/en/actions/using-workflows
- Pull request: https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#pull_request
- Syntax on.push: https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#onpushbranchestagsbranches-ignoretags-ignore
- Filter pattern cheat sheet: https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#filter-pattern-cheat-sheet


Items covered in the course are bellow: 

This course covers witch set of filters (event types) we can add to a event listener for a workflow

![](gh-event.png?raw=true)

- Only collaborator are eligible to activate the workflow even it maches with the events and filters inserted
- If the person who opened the PR is not a collaborator the workflow will keep pending until the owner approve it.

![](collaborator.png?raw=true)

- For example:

![](approve.png?raw=true)