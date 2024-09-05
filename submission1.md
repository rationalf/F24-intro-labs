# Benefits of signing commits

## Security

Signed commits confirm the identity of the developer. It is doesn't allow editing unauthorized user. It is helpful for open-source repositories.

## Workability

Signed commits give information about developer for his team, and help in understanding team distribution in big project

# Merge Strategies

## Standard Merge

When merging, Git tries to integrate changes from one branch into another. When it happens creats merge commits. Usually it is using when on one project work more than one people

## Squash and Merge

In Git, squash compress several commits into one. It give better possibility for reading commits in project.
In Git, Merge integrate changes from one branch into another, but when developers use Squash and Merge Git compress all commits in feature branch into one (Squash) before merging

## Rebase and Merge

Rebase it is alternative type of merging, when using Rebase Git put changes from one branch into another by replaying the changes from one branch on top of another without creating merge commit

