# Developer Documentation 

## Setting up your development repository

* Login to your github account and fork the main repository [mindfulness-at-the-computer](https://github.com/SunyataZero/mindfulness-at-the-computer)
* Make a clone of your new fork on your development environment and add remote `upstream` pointing to `git@github.com:SunyataZero/mindfulness-at-the-computer.git`. 
* [Configure your development environment](docs/configure_dev_env.md) to support running the application locally.
* Change directory into the top level of your clone.
* Execute 'make test'. (NOTE: This has not been implemented yet.)
* When you see all tests have passed, you are ready to start making code changes.

## Making Code Changes

### Find the issue you on which you will work. or create an issue to describe the work you plan to do.

### Sync with upstream and create a local branch for working on the issue. For example you might call the new branch `work_issue_96`.

### Simple Development Loop

Assumes automatic rebase on pull request merge not have any conflicts (it will be a fast-forward merge).

1. Make code changes, add new tests or fix tests that need to change.
2. Make sure automated tests pass locally.
3. Commit changes and push to your fork (`git push origin work_issue_96`).
4. Verify that Travis CI tests on your fork passed.
5. If more changes are needed, go to step 1, otherwise 
6. Sync with upstream and push to origin and verify Travis CI tests still pass.
7. Create a `pull request` to have the branch in your fork merged onto the main repository `master` branch.

### Development Loop with local rebase

Perfom local rebase regularly so that any conflicts are handled before requesting a pull request.

1. Make code changes, add new tests or fix tests that need to change.
2. Make sure automated tests pass locally.
3. Commit changes and push to your fork (`git push origin work_issue_96`).
4. Verify that Travis CI tests on your fork passed.
5. Sync with upstream, rebase onto master, push to origin and verify Travis CI tests still pass.
6. If more changes are needed, go to step 1, otherwise create a `pull request` to have the branch in your fork merged onto the main repository `master` branch.

## [Running from source](running-from-source.md)

## Useful links
* Link to [Travis CI Build and Test Results](https://travis-ci.org/SunyataZero/mindfulness-at-the-computer)
* Line to [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
