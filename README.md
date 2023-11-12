# Avail Chart

### Pre-requisites

#### Pre-commit

This repository uses the [pre-commit](https://pre-commit.com/) tool to manage linting, validation and generation of documentation. It does this using git hooks that must be installed locally on your repository

1. Install pre-commit
1. Install hook dependencies:
    - [yamllint](https://yamllint.readthedocs.io/en/stable/quickstart.html#installing-yamllint)
1. Run `pre-commit install` on the repo root to install the hooks

After installing every time you add a new commit the hooks will run, either passing or failing, depending if your code is compliant with the configurations.

Some hooks automatically fix the files for you and others only report the reason for failure and you will need to update the files yourself. After the problems have been fixed, you will only need to `git add/commit` them again until all the checks pass and the commit is registered.

You must use pre-commit when submitting new code. This is important to simplify code review and maintain a quality standard for the codebase.
