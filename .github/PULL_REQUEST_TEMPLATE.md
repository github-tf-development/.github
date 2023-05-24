# Platform Standards Pull Request
## Summary of what this Pull Request (PR) changes.

**IMPORTANT: Please do not create a Pull Request without creating an issue first.**

*Any change needs to be discussed before proceeding. Failure to do so may result in the rejection of the pull request.*

Please provide enough information so that others can review your pull request:

<!-- You can skip this if you're fixing a typo or adding an app to the Showcase. -->

Explain the **details** for making this change. What existing problem does the pull request solve?

<!-- Example: When "Adding a function to do X", explain why it is necessary to have a way to do X. -->

**Test plan (required)**

Demonstrate the code is solid. Example: The exact commands you ran and their output, screenshots / videos if the pull request changes UI.

<!-- Make sure tests pass on both Travis and Circle CI. -->

**Code formatting**

make sure to run tflint, tfvalidate, tffmt on your local machine for terraform IaC prior committing code.

<!-- See the simple style guide. -->

**Closing issues**

Put `closes #XXXX` in your comment to auto-close the issue that your PR fixes (if such).

Also after merging code with dev branch make sure you raise another pr to merge code on prod

## PR Checklist

- [ ] Have you filled in the above section on what this PR does?
- [ ] Have you tested the changes locally by running/validation the code?
- [ ] Have you verified your code does not contains secret/access keys?
- [ ] Have you updated the CHANGELOG file?
- [ ] Does the PR title start with the GitHub Issue ID e.g. "issue-1 - description here"
- [ ] Have you merged the latest changes from main and fixed any conflicts before pushing again? (`git fetch && git merge origin/main`)
- [ ] Has the PR been linked to the GitHub Issue you were working on? (In the "Development" option on the right on the GUI.)
- [ ] Has the PR been linked to the "WIZ" GitHub Project? (In the "Projects option on the right on the GUI.)
- [ ] Have you raised PR to merge your changes into prod branch?


Below checks are WIP

- [ ] Have you notified appropriate reviewers e.g. in the Slack channel.
