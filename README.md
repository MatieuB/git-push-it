# Git Push-It

This is a simple git plugin that plays appropriate music while pushing your code.

This plugin requires `git > 1.8.2`.

## HTTP/HTTPS Remotes

Using this plugin with a remote via http/https, requires you to login with username and password _every time_ you push your code.

You must also enable caching with git's credential helper.

```bash
$ git config --global credential.helper cache
```

For more on credential caching with git, view the  [documentation](https://git-scm.com/docs/gitcredentials).

## Install

To install, simply copy and paste the following into your terminal.

```bash
$ git clone https://github.com/skuttleman/git-push-it.git ~/.git-push-it
$ ln -s ~/.git-push-it/git-push-it /usr/local/bin/git-push-it
```

## Update

To update to the latest version of git-push-it:

```bash
$ cd ~/.git-push-it; git pull; cd -
```

## Usage

It defaults to `origin master`, but will take a `<remote>` and `<branch>`.

```bash
$ git push-it
$ git push-it some-remote some-branch
```
