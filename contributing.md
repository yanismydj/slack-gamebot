# Contributing to SlackGamebot

This project is work of [many contributors](https://github.com/dblock/slack-gamebot/graphs/contributors).

You're encouraged to submit [pull requests](https://github.com/dblock/slack-gamebot/pulls), [propose features and discuss issues](https://github.com/dblock/slack-gamebot/issues).

In the examples below, substitute your Github username for `contributor` in URLs.

## Fork the Project

Fork the [project on Github](https://github.com/dblock/slack-gamebot) and check out your copy.

```text
git clone https://github.com/contributor/slack-gamebot.git
cd slack-gamebot
git remote add upstream https://github.com/dblock/slack-gamebot.git
```

## Create a Topic Branch

Make sure your fork is up-to-date and create a topic branch for your feature or bug fix.

```text
git checkout master
git pull upstream master
git checkout -b my-feature-branch
```

## Bundle Install and Test

Ensure that you can build the project and run tests.

```text
bundle install
bundle exec rake
```

## Write Tests

Try to write a test that reproduces the problem you're trying to fix or describes a feature that you want to build. Add to [spec](https://github.com/yanismydj/slack-gamebot/tree/146d4bd357f85826024e4d37e3c66859cbd6a71c/spec/README.md).

We definitely appreciate pull requests that highlight or reproduce a problem, even without a fix.

## Write Code

Implement your feature or bug fix.

Ruby style is enforced with [Rubocop](https://github.com/bbatsov/rubocop). Run `bundle exec rubocop` and fix any style issues highlighted.

Make sure that `bundle exec rake` completes without errors.

## Write Documentation

Document any external behavior in the [README](./).

## Update Changelog

Add a line to [CHANGELOG](changelog.md) under _Next Release_. Make it look like every other line, including your name and link to your Github account.

## Commit Changes

Make sure git knows your name and email address:

```text
git config --global user.name "Your Name"
git config --global user.email "contributor@example.com"
```

Writing good commit logs is important. A commit log should describe what changed and why.

```text
git add ...
git commit
```

## Push

```text
git push origin my-feature-branch
```

## Make a Pull Request

Go to [https://github.com/contributor/slack-gamebot](https://github.com/contributor/slack-gamebot) and select your feature branch. Click the 'Pull Request' button and fill out the form. Pull requests are usually reviewed within a few days.

## Rebase

If you've been working on a change for a while, rebase with upstream/master.

```text
git fetch upstream
git rebase upstream/master
git push origin my-feature-branch -f
```

## Update CHANGELOG Again

Update the [CHANGELOG](changelog.md) with the pull request number. A typical entry looks as follows.

```text
* [#123](https://github.com/dblock/slack-gamebot/pull/123): Reticulated splines - [@contributor](https://github.com/contributor).
```

Amend your previous commit and force push the changes.

```text
git commit --amend
git push origin my-feature-branch -f
```

## Check on Your Pull Request

Go back to your pull request after a few minutes and see whether it passed muster with Travis-CI. Everything should look green, otherwise fix issues and amend your commit as described above.

## Be Patient

It's likely that your change will not be merged and that the nitpicky maintainers will ask you to do more, or fix seemingly benign problems. Hang on there!

## Thank You

Please do know that we really appreciate and value your time and work. We love you, really.

