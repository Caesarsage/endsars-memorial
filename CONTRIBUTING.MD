# CONTRIBUTING

This document describes the steps you need to take to be able to contribute efficiently to this project.

## To contribute to this project, you should first of all

1. Fork the repository. Forking the repository creates a copy of this repository on your Github account. Fork this repositiory by clicking on the `Fork` button on this project's Github page

2. Clone your fork. By cloning your fork, you will eventually have a copy of the repository on your local computer.

3. After cloning to your local, set up the local repository to be linked with the upstream repository. The upstream repository is the reository that you forked from. This will enable you to update your local repository with the upstream repository from the comfort of your computer. Do this via the following process
  - Copy the Github URL of the upstream repositrory (which can be found on the clone button of the upstream repository)
  - Open a terminal in the cloned project's folder and run
  `git remote add upstream [URL_OF_UPSTREAM_REPOSITORY]`.
  - Run `git remote -v` on your terminal to verify that the upstream repository has been added. You will see the upstream repository and its Github URL if it has been added.

4. Create and switch to a new branch from which you'll be working from using `git checkout -b [NEW_BRANCH_NAME]` . This is important so that your work can be separate from what is already existing on the repository and won't cause branch-related conflicts when your work is merged


## Doing your work

1. Do your work on the new branch which you've switched/checked out to and make your commits when you are done.

## Syncing your local repository with the upstream repository

It is good to update yor work with the current state of the upstream repostory before making a pull request that your work should be merged. This ensures that you are not submitting past work alongside the good work that you have done, and then cause previous work to override current work on the project.

To sync your local repository with the upstream repository,

1. Make sure that you have commited your latest work locally.

2. On your terminal, run `git pull upstream develop`. This will get the latest work on the upstream repository's `develop` branch and combine it with what you have on your local. If there are any conflicts, choose the work from `upstream develop` over the work on your local for files that you're not supposed to work on. Do otherwise for files that you worked on.

## Submitting your work/Making a pull request

Please make sure your work is up-to-date by following the steps in [Syncing your local repository with the upstream repository](#Syncing-your-local-repository-with-the-upstream-repository) before making a pull request. To make a pull request,

1. Push the latest work on the branch you worked on to your remote (origin) repository, and make a pull request to the upstream repository's `develop` branch. Always make PRs to the `develop` branch.

2. Please include a commit message title and a body so that whoever is verifying the work will have heads-on on what the work is about.

Thak you