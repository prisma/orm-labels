# orm-labels

This repository is only used to configure [GitHub labels](../../labels), which are then copied over to new repositories.

## How to use


### Prerequisites

- Install GitHub CLI: https://github.com/cli/cli#installation
- Run `gh auth login`

### First, check the labels on the destination repository
 
Go to the repository where you want to copy the labels, https://github.com/prisma/%my-destination-repo%/labels and delete unwanted labels.

### Second, copy the labels to the destination repository

Using the command below, copy the [existing labels of this repository](../../labels) to the repository defined, here `prisma/my-destination-repo` as an example:

```
gh label clone prisma/orm-labels --repo prisma/my-destination-repo
! Cloned 35 labels of 44 from prisma/orm-labels to prisma/my-destination-repo
```

See https://cli.github.com/manual/gh_label_clone documentation for more information.
