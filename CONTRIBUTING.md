# Contributing to Ransack

Please take a moment to review this document in order to make the contribution
process easy and effective for everyone involved!

Ransack is an open source project and we encourage contributions.

## Filing an issue

A bug is a _demonstrable problem_ that is caused by the code in the repository.
Good bug reports are extremely helpful!

Guidelines for bug reports:

1. **Use the GitHub issue search** &mdash; check if the issue has already been
   reported.

2. **Check if the issue has been fixed** &mdash; try to reproduce it using the
   `master` branch in the repository.

3. **Isolate and report the problem** &mdash; ideally create a reduced test
   case.

When filing an issue, please provide these details:

* A comprehensive list of steps to reproduce the issue, or - far better - **a failing spec**.
* The version (and branch) of Ransack *and* the versions of Rails, Ruby, and your operating system.
* Any relevant stack traces ("Full trace" preferred).

Any issue that is open for 14 days without actionable information or activity
will be marked as "stalled" and then closed. Stalled issues can be re-opened
if the information requested is provided.

## Pull requests

We gladly accept pull requests to fix bugs and, in some circumstances, add new
features to Ransack.

Before issuing a pull request, please make sure that all specs are passing,
that any new features have test coverage, and that anything that breaks
backward compatibility has a very good reason for doing so.

Here's a quick guide:

1. Fork the repo.

2. Run the tests. We only take pull requests with passing tests, and it's great
to know that you have a clean slate:

        $ bundle install
        $ bundle exec rake spec

3. Add a test for your change. Only refactoring and documentation changes
require no new tests. If you are adding functionality or fixing a bug, we need
a test!

4. Make the test pass.

5. Push to your fork and submit a pull request. If the changes will apply
cleanly to the latest stable branches and master branch, you will only need
to submit one pull request.

6. If your pull request only contains documentation changes, please remember to
add `[skip ci]` to your commit message so the Travis test suite doesn't run
needlessly.

At this point you're waiting on us. We like to at least comment on, if not
accept, pull requests within three business days (and, typically, one business
day). We may suggest some changes or improvements or alternatives.

Some things that will increase the chance that your pull request is accepted,
taken straight from the Ruby on Rails guide:

* Use Rails idioms and helpers.
* Include tests that fail without your code, and pass with it.
* Update the README, the change log, the wiki documentation... anything that is
  affected by your contribution.

Syntax:

* Two spaces, no tabs.
* 80 characters per line.
* No trailing whitespace. Blank lines should not have any space.
* Prefer `&&`/`||` over `and`/`or`.
* `MyClass.my_method(my_arg)` not `my_method( my_arg )` or my_method my_arg.
* `a = b` and not `a=b`.
* `a_method { |block| ... }` and not `a_method { | block | ... }` or
`a_method{|block| ...}`.
* Follow the conventions you see used in the source already.

And in case we didn't emphasize it enough: we love tests!
