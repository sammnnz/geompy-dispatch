# geompy-dispatch
GitHub Action's workflows for remote call workflows from [geompy](https://github.com/sammnnz/geompy/) repo.

### How?
Here, using two types of workflow's run:
* Call [reusable workflows](https://docs.github.com/en/actions/sharing-automations/reusing-workflows) (with `workflow_call` events);
* Using [GitHub CLI in workflows](https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/using-github-cli-in-workflows) (see [create dispatch event](https://docs.github.com/en/rest/actions/workflows?apiVersion=2022-11-28#create-a-workflow-dispatch-event)).

### Why?
There is a good answer on [stackoverflow](https://stackoverflow.com/questions/67523882/workflow-is-not-shown-so-i-cannot-run-it-manually-github-actions/71423764#71423764).
In short, some workflows (based on `workflow_dispatch` event) will not even show until the code is on the main (or default branch).