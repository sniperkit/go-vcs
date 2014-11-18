go-vcs - manipulate and inspect VCS repositories
================================================

go-vcs is a library for manipulating and inspecting VCS repositories in Go. It currently supports
Git and Mercurial (hg).

Note: the public API is experimental and subject to change until further notice.

* [Documentation on Sourcegraph](https://sourcegraph.com/sourcegraph.com/sourcegraph/go-vcs)

[![Build Status](https://travis-ci.org/sourcegraph/go-vcs.png?branch=master)](https://travis-ci.org/sourcegraph/go-vcs)
[![status](https://sourcegraph.com/api/repos/sourcegraph.com/sourcegraph/go-vcs/.badges/status.png)](https://sourcegraph.com/sourcegraph.com/sourcegraph/go-vcs)


Installing
==========

```
go get -u sourcegraph.com/sourcegraph/go-vcs/vcs
```

To use the faster libgit2 implementation of git, install git2go (run
`make install` in its repository root) first. You also need to install
libssh2 for SSH support.

For hg blame, you need to install hglib: `pip install hglib`.


Running tests
=============

Run `go test ./vcs/...`. Note that the tests test the libgit2
implementation and SSH support (see above instructions).


Contributors
============

* Quinn Slack <sqs@sourcegraph.com>
