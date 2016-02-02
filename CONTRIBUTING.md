# Contributing to Lelylan

This document tries to define a contributor's guide explaining how to contribute to one or more Lelylan Microservices. 
It contains information about reporting issues as well as some tips and guidelines useful to experienced open source 
contributors.


### Topics

* [General Issues](#general-issues)
* [Security Issues](#security-issues)
* [Design Proposals](#design-proposals)
* [Tips and guidelines](#tips-and-guidelines)
* [Community Guidelines](#community-guidelines)



# General Issues

A good way to contribute to an open source project is to send a detailed report when you encounter an issue. 
We appreciate a well-written, thorough bug report, and will thank you for it in advance for your help

Check that [our main issue database](https://github.com/lelylan/lelylan/issues) or the issue related to a specific
microservice doesn't already include that problem or suggestion before submitting an issue. If you find a match, 
you can use the "subscribe" button to get notified on updates. Try to not leave random "+1" or "I have this too" 
comments (they don't add useful information). Instead if you have ways to reproduce the issue or have additional 
information that may help resolving the issue, please leave a comment.

Include the steps required to reproduce the problem if possible and applicable. This information will help us 
review and fix the issue faster. When sending lengthy log-files, consider posting them as a [gist](https://gist.github.com).
Don't forget to remove sensitive data from your logfiles before posting (you can replace those parts with "REDACTED").

When reporting issues try to include the following elements

* The language version (`ruby -v` or `node -v`)
* Environment details (e.g. local, AWS, VirtualBox, physical)
* Steps to reproduce the issue
* Actual results
* Expected results
* Additional info



# Security issues

Security is an important topic in the Internet of Things. If you discover a security issue, please bring it to 
our attention right away. Please do not file a public issue. Instead send your report privately to 
[dev@lelylan.com](mailto:dev@lelylan.com).

Security reports are greatly appreciated and we will publicly thank you for it. We currently do not offer a paid 
security bounty program, but we hope to start in the near future.



# Design proposals

You can propose new designs for existing Lelylan features. You can also design entirely new features. We really 
appreciate contributors who want to refactor or otherwise cleanup the project. We try hard to keep Lelylan lean 
and focused. Lelylan can't do everything for everybody. This means that we might decide against incorporating a 
new feature. However, there might be a way to implement that feature on top of Lelylan or creating an additional 
microservice.

A refactor or cleanup proposal changes Lelylan’s internal structure without altering the external behavior. 
To make this type of proposal:

* Fork the desired microservice.
* Make your changes in a feature branch.
* Sync and rebase with master as you work.
* Run the full test suite.
* Submit your code through a pull request (PR).
* The PR’s title should be clear (e.g. Cleanup: defined acceptance shared tests).
* Refine your proposal through review (maintainers and community review your proposal).
* Acceptance and merge.

If your changes required logic changes, note that in your request.



# Tips and guidelines

This section gives the experienced contributor some tips and guidelines.


### Pull requests are always welcome

Not sure if that typo is worth a pull request? Found a bug and know how to fix it? Please do it. We will appreciate it. 
Any significant improvement should be documented as [a GitHub issue](https://github.com/lelylan/lelylan/issues) before
anybody starts working on it.

We are always thrilled to receive pull requests. We do our best to process them quickly. If your pull request is not 
accepted on the first try, don't get discouraged and try to use the received feedback to refine your contribution.

### Talking to the Lelylan community

Get in touch with the community through the [support](http://dev.lelylan.com/support) page.


### Conventions

Fork the repository and make changes on your fork in a feature branch.

- If it's a bug fix branch, name it XX-something where XX is the number of the issue. 
- If it's a feature branch, create an enhancement issue to announce your intentions, and name it XX-something 
where XX is the number of the	issue.

Submit unit tests for your changes. Ruby and Node.js have great test frameworks. Take a look at existing tests 
for inspiration. Run the full test suite on your branch before submitting a pull request.

Update the documentation when creating or modifying features. Test your documentation changes for clarity, 
concision, and correctness, following the [Docker guidelines](https://docs.docker.com/opensource/doc-style/).
Changes are made to the [dev center repo](https://github.com/lelylan/dev).

Pull request descriptions should be as clear as possible and include a reference to all the issues that they address.
Commit messages must start with a capitalized and short summary (max. 50 chars) written in the imperative, followed 
by an optional, more detailed explanatory text which is separated from the summary by an empty line.

Code review comments may be added to your pull request. Discuss, then make the suggested modifications and push 
additional commits to your feature branch. Post a comment after pushing. New commits show up in the pull request 
automatically, but the reviewers are notified only when you comment. 

Before you make a pull request, squash your commits into logical units of work using `git rebase -i` and 
`git push -f`. A logical unit of work is a consistent set of patches that should be reviewed together: 
for example, upgrading the version of a vendored dependency and taking advantage of its now available new
feature constitute two separate units of work. Implementing a new function and calling it in another file 
constitute a single logical unit of work. The very high majority of submissions should have a single commit, 
so if in doubt: squash down to one. Include an issue reference like `Closes #XX` in commits that close an issue. 
Including references automatically closes the issue on a merge.


### Merge approval

Lelylan maintainers use LGTM (Looks Good To Me) in comments on the code review to indicate acceptance. A change 
requires LGTMs from an absolute majority of the maintainers of each component affected. For example, if a change 
affects `dev/` and `devices/`, it needs an absolute majority from the maintainers of `dev/` AND, separately, an
absolute majority of the maintainers of `devices/`.


## Lelylan community guidelines

We want to keep the Lelylan community active, growing and collaborative. We need your help to keep it that way. 
To help with this we've come up with some general guidelines for the community as a whole:

* Be nice. Be courteous, respectful and polite to fellow community members:
  no regional, racial, gender, or other abuse will be tolerated.

* Encourage diversity and participation. Make everyone in our community feel
  welcome, regardless of their background and the extent of their
  contributions, and do everything possible to encourage participation in
  our community.

* Keep it legal. Basically, don't get us in trouble. Share only content that
  you own, do not share private or sensitive information, and don't break
  the law.

* Stay on topic. Make sure that you are posting to the correct channel and
  avoid off-topic discussions. Remember when you update an issue or respond
  to an email you are potentially sending to a large number of people. Please
  consider this before you update. Also remember that nobody likes spam.

* Don't send email to the maintainers. There's no need to send email to the
  maintainers to ask them to investigate an issue or to take a look at a
  pull request. Instead of sending an email, GitHub mentions should be
  used to ping maintainers to review a pull request, a proposal or an
  issue.


### Guideline violations — 3 strikes method

The point of this section is not to find opportunities to punish people, but we
do need a fair way to deal with people who are making our community suck.

1. First occurrence: we'll give you a friendly, but public reminder that the
   behavior is inappropriate according to our guidelines.

2. Second occurrence: we will send you a private message with a warning that
   any additional violations will result in removal from the community.

3. Third occurrence: depending on the violation, we may need to delete or ban
   your account.


### Notes

* Obvious spammers are banned on first occurrence. If we don't do this, we'll
  have spam all over the place.

* Violations are forgiven after 6 months of good behavior, and we won't hold a
  grudge.

* People who commit minor infractions will get some education, rather than
  hammering them in the 3 strikes process.

* The rules apply equally to everyone in the community, no matter how much
	you've contributed.

* Extreme violations of a threatening, abusive, destructive or illegal nature
	will be addressed immediately and are not subject to 3 strikes or forgiveness.

* Contact dev@lelylan.com to report abuse or appeal violations. In the case of
	appeals, we know that mistakes happen, and we'll work with you to come up with a
	fair solution if there has been a misunderstanding.


## Coding Style

Unless explicitly stated, we follow the coding guidelines from the Ruby and Node.js community.

It is possible that the code base does not currently comply with these guidelines. We are not looking for a massive 
PR that fixes this, since that goes against the spirit of the guidelines. All new contributions should make a
best effort to clean up and make the code base better than they left it. Obviously, apply your best judgement. 
Remember, the goal here is to make the code base easier for humans to navigate and understand. Always keep that 
in mind when nudging others to comply.

* [Ruby coding guidelines](https://github.com/styleguide/ruby)
* [Node.js coding guidelines](https://github.com/felixge/node-style-guide)
