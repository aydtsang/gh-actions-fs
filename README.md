# Learning Github Actions From scratch

TODO:
- LINK TO RECORDING

This repo is a documented guide to learning Github Actions from scratch.

## The Plan

Intuitively, the first thing we should do is check whether or not Github has
already published a guide on learning Github Actions.

You can find it here - https://docs.github.com/en/actions/learn-github-actions

Github Actions allows you to automate tasks that are normally run throughout the
development process (i.e. build, test, deploy).

## Concepts
- _Events_
- _Workflows_
- Sequential or Parallel _Jobs_
- Virtual Machine or Container _Runner_

### Workflows
> A workflow is a configurable automated process that will run one or more jobs. 
Workflows are defined by a YAML file checked in to your repository and will run 
when triggered by an event in your repository, or they can be triggered manually, 
or at a defined schedule.

Key Points:
- Workflows are defined in the `.github/workflows` directory in a repository
- A repository can have multiple workflows
- You can reference a workflow within another workflow

[Using Workflows](https://docs.github.com/en/actions/using-workflows)

### Events
An event is a specific activity in a repository that triggers a workflow run.

List of [supported events](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows)

### Jobs
> A job is a set of steps in a workflow that execute on the same runner. 

- Each step is either a shell script or an "action" 
- Each step is executed on the same runner
- Share data from one step to another

[Using Jobs](https://docs.github.com/en/actions/using-jobs)
