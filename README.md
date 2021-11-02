# Git Collaboration Guide

## 1. Assign a team member to create a GitHub repository

The assigned team member is also responsible for changing the initial settings for the repository. See [here](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features) for documentation on managing the features and settings of a GitHub repository.

After the team member has created the repository, they should share the GitHub URL with the other team members.

## 2. Clone the repository

Every team member should clone the repository. If an individual uses multiple computers, they should clone the repository to each separately.

## 3. Create branches

A team member should create a new branch for a distinct item of work, e.g., cleaning a dataset, or implementing a regression, etc. Such a branch is called a "*topic branch*". If multiple people contribute to a single item of work, the group should assign an individual to create the topic branch on the GitHub repository (one may also create the branch locally and then push to the GitHub repository).

An individual should checkout the topic branch to make changes relevant to the item of work. If multiple people contribute to the item, each should create another branch based on the topic branch.

## 4. Commit logically related changes

A commit may include changes to multiple files as long as the changes are all logically related. If a branch represents a high-level item of work, then a commit represents the completion of a discrete task that is part of that item of work. For example, in a branch dedicated to preparing the input for a model, the addition of a new .CSV file containing a dataset, and the implementation of new code to read the dataset into a variable may go into the same commit. Additional code to process the data should be saved to a separate commit.

One should also consider the potential for reverting to a previous state of the project when making a commit. Answer the question "would I (or a teammate) want to roll back a subset of these changes and keep the rest?" before committing. If the answer is yes, then you should only include the changes that would be rolled back together in the commit.
