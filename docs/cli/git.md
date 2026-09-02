---
icon: material/console-line
title: GitOps
---

# GitOps

To clone a repo:

```bash
# Cloning with git via HTTPS
git clone https://github.com/myseq/tracker

# Cloning with git via SSH
git clone git@github.com:myseq/tracker.git

# Cloning with GH
gh repo clone tracker

```

To rename/set origin URL: `git remote set-url origin git@github.com:myseq/tracker.git`



## Workflow

To list all available workflows: `gh workflow list`

To create a workflow_dispatch event for `updater.yml` at `main`: `gh workflow run updater.yml`

### repo:tracker

To run one of the workflow: `gh workflow run 266672972`

To show all the workflow outputs: `gh run list --workflow=updater.yml`

### repo:github.io

To run one of the workflow: `gh workflow run 71647049`

To show all the workflow outputs: `gh run list --workflow=hugo.yaml`


## New Repo

 1. Login GH: `gh auth login`
 1. Verify login status: `gh auth status`
 1. Navigate to existing project folder.
 1. Initialize Git locally: `git init`
 1. Stage and commit: 


 1. Rename default branch to `main` (`master`): `git branch -M main`
 1. Create the private repo and upload:

```console
% gh repo create my-private-repo --private --source=. --push
```

 1. (In case) To create a public repo and upload:

```console
% gh repo create my-public-repo --public --source=. --push
```

 1. Verify the upload: `gh repo view --web`


