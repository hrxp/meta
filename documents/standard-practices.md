# Standard practices

Almost everything here is a _guideline_. Don't be afraid to bend or break them if you can articulate a clear reason to.

## Code

* Format your code using [Prettier](https://prettier.io).
* Take advantage of [modern JavaScript syntax](http://es6-features.org/).
* Design applications that adhere to the [Twelve-Factor App](https://12factor.net) methodology.

## Version control

_Inspired by [jbenet's "simple branching model"](https://gist.github.com/jbenet/ee6c9ac48068889b0912)._

#### Branches

* `master` is the main branch of the repository. It has special qualities:
  * it should always be deployable (i.e.,, never break master!).
  * it should never be committed to directly -- pull requests are the mechanism for introducing changes.
* Feature branches should be branched from `master`, and pull requests to merge
  feature branches should be opened against `master`.
* There's no need to maintain your own fork, you can just push your feature
  branches directly.

#### Pull requests
* A pull request should be a set of related changes -- don't sneak unrelated
  modifications in.
  * Clean, narrow PRs make it easier to reason about bugs and commit history.
  * Err on the side of opening too many PRs, rather than not enough.
* Include a description that mentions: 
  * a summary of what your PR includes
  * a description of your approach
  * commentary on the larger story around your PR

#### Commits

* Commits should be reasonably [atomic](ttps://seesparkbox.com/foundry/atomic_commits_with_git).
* Commit messages should follow the [Conventional
  Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.2/) standard.
  * E.g.: `feat: user login flow` or `fix: navbar styling in Safari 11`
* Limit your subject (first) line to 70 characters (GitHub truncates more than this).
* Provide a body if you'd like to explain your commit in detail.
* Your subject line should complete this sentence: `If applied, this commit will [your subject line]`.
* Recommended reading:
  * ["The seven rules of a great Git commit message"](https://chris.beams.io/posts/git-commit/#seven-rules)

#### Releases
* Releases should only ever be made from the tip of `master`.
* Releases to production should be tracked using git tags and [GitHub Releases](https://help.github.com/en/articles/creating-releases).
