# Revolution Pi

## Sunsetting our presence on GitHub

In September of 2023 Revolution Pi has moved all git repositories to GitLab. The
Revolution Pi GitLab organization can be found at the following address:

https://gitlab.com/revolutionpi/.

To minimize the impact for users of the repositories on GitHub we decided to
mirror all repositories from GitLab to GitHub, but after more than 2 years we've
made the decision to sunset our presence on GitHub. All repositories on GitHub
will be archived in Q1 of 2026 and will thus no longer be updated either.  This
also means we will only accept contributions through GitLab going forward.

Tracking the GitLab repositories instead of the GitHub ones requires a small
change in git. The git-remote(1) command is used to change the URL where the
repository is available. For example, assuming that the remote is named `origin`
and the repository is `linux`:

```
git remote set-url origin https://gitlab.com/revolutionpi/linux.git
```