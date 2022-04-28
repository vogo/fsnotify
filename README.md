# WARNING

**This is a fork of github.com/fsnotify/fsnotify, enable configuring watch event as you wish.**

[![GoDoc](https://godoc.org/github.com/fsnotify/fsnotify?status.svg)](https://godoc.org/github.com/fsnotify/fsnotify) [![Go Report Card](https://goreportcard.com/badge/github.com/fsnotify/fsnotify)](https://goreportcard.com/report/github.com/fsnotify/fsnotify)
=======
If you are reading this, you use `master` branch of this repository,
which is wrong.

This branch
 - should not be used;
 - is not maintained;
 - is not supported;
 - will be removed soon.

You should switch to using the default branch instead.

## Using git

Here's how to switch your existing local copy of this repository from `master`
to `main` (assuming the remote name is `origin`):

```
git branch -m master main
git fetch origin
git branch -u origin/main main
git remote set-head origin -a
```

In addition to the above, if you want to remove the leftover `origin/master`
remote branch (NOTE this also removes all other remote branches that no longer
exist in `origin`):

```
git remote prune origin
```

## Background

The `master` branch was renamed to `main`, causing an issue with
Yocto/OpenEmbedded's meta-virtualization layer, which explicitly refers
to `master` branch of this repository (see #426).

This temporary branch is created to alleviate the Yocto/OE issue.
