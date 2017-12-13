# Developer Documentation 

## Getting Started
* Login to your github account and fork the main repository
  [mindfulness-at-the-computer](https://github.com/SunyataZero/mindfulness-at-the-computer)
* Make a clone of your new fork on your development environment.
* [Configure your development environment](docs/configure_dev_dnv.md) to support running the application locally.
* Change directory into the top level of your clone.
* Execute 'make test'.
* When you see all tests have passed, you are ready to start making code changes.

## Making Code Changes
* Find the issue you on which you will work. or create an issue to describe the work you plan to do.
* Sync with upstream and create a local branch for working on the issue. For example you might call the new branch `work_issue_96`.
* Development Loop
1. Make code changes, add new tests or fix tests that need to change.
2. Make sure automated tests pass locally.
3. Commit changes and push to your fork (`git push origin work_issue_96`).
4. Verify that Travis CI tests on your fork passed.
5. Sync with upstream, rebase onto master, push to origin and verify Travis CI tests still pass.
6. If more changes are needed, go to step 1, otherwise create a `pull request` to have the branch in your fork merged
   onto the main repository `master` branch.

## [Running from source](running-from-source.md)

## Useful links
* Link to [Travis CI Build and Test Results](https://travis-ci.org/SunyataZero/mindfulness-at-the-computer)
* Line to [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
