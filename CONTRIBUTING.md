## Contributing to LFS Test Server

Hi there! We're thrilled that you'd like to contribute to this project. Your
help is essential for keeping it great.

Contributions to this project are [released](https://help.github.com/articles/github-terms-of-service/#6-contributions-under-repository-license) to the public under the [project's open source license](LICENSE).

## Submitting a pull request

0. [Fork][] and clone the repository
0. Configure and install the dependencies: `go build`
0. Make sure the tests pass on your machine: `go test`
0. Create a new branch: `git checkout -b my-branch-name`
0. Make your change, add tests, and make sure the tests still pass
0. Push to your fork and [submit a pull request][pr]
0. Pat your self on the back and wait for your pull request to be reviewed.

Here are a few things you can do that will increase the likelihood of your pull request being accepted:

- Follow the [style guide][style] where possible.
- Write tests.
- Update documentation as necessary.
- Keep your change as focused as possible. If there are multiple changes you
would like to make that are not dependent upon each other, consider submitting
them as separate pull requests.
- Write a [good commit message](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).

## Updating management templates
0. Install go.rice with `go install github.com/GeertJohan/go.rice`
0. Run `rice embed-go` after all template changes have been made
0. Commit the change
0. Submit a pull request.

## Updating 3rd party packages

0. Run `godep save` to add new dependencies.
0. Run `godep update foo/bar` to update the package `foo/bar`.
0. Commit the change.  lfs-test-server vendors the full source code in the repository.
0. Submit a pull request.

## Resources

- [Contributing to Open Source on GitHub](https://guides.github.com/activities/contributing-to-open-source/)
- [Using Pull Requests](https://help.github.com/articles/using-pull-requests/)
- [GitHub Help](https://help.github.com)

[![GoDoc](https://godoc.org/github.com/github/lfs-test-server?status.svg)](https://godoc.org/github.com/github/lfs-test-server)

[fork]: https://github.com/github/lfs-test-server/fork
[pr]: https://github.com/github/lfs-test-server/compare
[style]: https://github.com/golang/go/wiki/CodeReviewComments
