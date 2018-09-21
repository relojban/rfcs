# Relojban RFCs
[Relojban RFCs]: #relojban-rfcs

**Attention: the process described below should be taken as a suggestion of good practices to adopt once (if) a stable and self-sustaining Relojban community exists. It might take a while. In the meantime the strategy will be inevitably [flexible](https://en.wiktionary.org/wiki/fly_by_the_seat_of_one%27s_pants).**


## Introduction
[Introduction]: #introduction

Many changes, such as bug fixes or improvements to the dictionary and documentation, can be implemented and reviewed via the normal GitHub pull request workflow.

Some changes though are "substantial", and we ask that these be put through a bit of a design process to make sure Relojban progresses in a coherent direction in line with the consensus of the community.

The "RFC" (request for comments) process is intended to provide a consistent and controlled path for new features to enter the language and the software built around it, so that everyone involved can be confident about the dirction of the project.


## Table of Contents
[Table of Contents]: #table-of-contents

  - [When you need to follow this process]
  - [Before creating an RFC]
  - [What the process is]
  - [The RFC life-cycle]
  - [License]


## When you need to follow this process
[When you need to follow this process]: #when-you-need-to-follow-this-process

You need to follow this process if you intend to make "substantial" changes to the Relojban book, the dictionary, the parsers, or the RFC process itself. What constitutes a "substantial" change is evolving based on community norms, but may include the following.

  - Any semantic or syntactic change to the language that is not a bugfix.
  - Changes to the place structures of words in the dictionary.
  - Changes touching the main interfaces and data structures of the parsers or of the other software tools.

Some changes do not require an RFC. In particular no RFC is expected for rephrasing, reorganizing, refactoring, or otherwise "changing shape without changing meaning".

If you submit a pull request to implement a "substantial" change without going through the RFC process, it may be closed with a polite request to submit an RFC first.


## Before creating an RFC
[Before creating an RFC]: #before-creating-an-rfc

A hastily-proposed RFC can hurt its chances of acceptance. Low quality proposals, proposals for previously-rejected features, or those that don't match with the long-term goals of the project, may be quickly rejected, which can be demotivating for the unprepared contributor. Laying some groundwork ahead of the RFC can make the process smoother.

Although there is no single way to prepare for submitting an RFC, it is generally a good idea to pursue feedback from other project members beforehand, to ascertain that the RFC may be desirable. The most common preparations for writing and submitting an RFC include discussing the topic on the [mailing list](https://www.relojban.org/participate/), possibly posting "pre-RFCs" to gather feedback.

As a rule of thumb, receiving encouraging feedback from long-standing project maintainers is a good indication that the RFC is worth pursuing.


## What the process is
[What the process is]: #what-the-process-is

In short, to get a major change into Relojban, one must first get the RFC merged into the RFC repository as a markdown file. This signals that the change is to be pursued. From that point on, the RFC is "active" and may be implemented throughout the project repositories (in the book, in the parsers, etc. ).

  - Fork the [RFC repository](http://github.com/relojban/rfcs)
  - Copy `0000-template.md` to `text/0000-my-proposal.md` (where "my-proposal" is descriptive). Don't assign an RFC number yet.
  - Fill in the RFC. Put care into the details: RFCs that do not present convincing motivation, demonstrate understanding of the impact of the design, or are disingenuous about the drawbacks or alternatives tend to be poorly-received.
  - Submit a pull request. As a pull request the RFC will receive design feedback from the larger community, and the author should be prepared to revise it in response.
  - Build consensus and integrate feedback. RFCs that have broad support are much more likely to make progress than those that don't receive any comments.
  - The discussion of the RFC should take place as much as possible in the comment thread of the pull request itself, and should be kept strictly on topic.
  - RFCs rarely go through this process unchanged, especially as alternatives and drawbacks are shown. You can make edits, big and small, to the RFC to clarify or change the design, but make changes as new commits to the pull request, and leave a comment on the pull request explaining your changes. Specifically, do not squash or rebase commits after they are visible on the pull request.
  - At some point, a Relojban maintainer will propose a "motion for final comment period" (FCP), along with a *disposition* for the RFC (merge or close).
  - This step is taken when enough of the tradeoffs have been discussed that the maintainers are in a position to make a decision. That does not require consensus amongst all participants in the RFC thread (which is usually impossible). However, the argument supporting the disposition on the RFC needs to have already been clearly articulated, and there should not be a strong consensus *against* that position outside of the maintainers.
  - Maintainers use their best judgment in taking this step, and the FCP itself ensures there is ample time and notification for stakeholders to push back if it is made prematurely.
  - Before actually entering FCP, *all* maintainers must sign off (how they reach such unanimity is left to them);
  - The FCP lasts ten calendar days, so that it is open for at least 5 business days. During this period, it is advertised widely across the community. This way all stakeholders have a chance to lodge any final objections before a decision is reached.
  - In most cases, the FCP period is quiet, and the RFC is either merged or closed. However, sometimes substantial new arguments or ideas are raised, the FCP is canceled, and the RFC goes back into development mode.


## The RFC life-cycle
[The RFC life-cycle]: #the-rfc-life-cycle

Once an RFC becomes "active" then authors may implement it and submit the changes as pull requests to the appropriate repositories. Being "active" is not a rubber stamp, and in particular still does not mean the proposal will ultimately be merged; it does mean that in principle all the major stakeholders have agreed to the proposal and are amenable to merging it.

Furthermore, the fact that a given RFC has been accepted and is "active" implies nothing about what priority is assigned to its implementation, nor does it imply anything about whether a Relojban maintainer has been assigned the task of implementing the proposal. While it is not *necessary* that the author of the RFC also write the implementation, it is by far the most effective way to see an RFC through to completion: authors should not expect that other project maintainers will take on responsibility for implementing their proposal.

Modifications to "active" RFCs can be done in follow-up pull requests. In general, once accepted, RFCs should not be substantially changed. Only very minor changes should be submitted as amendments. More substantial changes should be new RFCs, with a note added to the original RFC.


## License
[License]: #license

The Relojban RFC process is an adaptation of the [Rust RFC process](https://github.com/rust-lang/rfcs/), which is licensed under either the MIT or the Apache 2.0 license.

Any content in this repository that is not a derivative work is dedicated to the public domain under the terms of the [Unlicense](UNLICENSE) (see <http://unlicense.org>).

For any contribution intentionally submitted for inclusion to this repository, the submitter agrees to dedicate any and all copyright interest to the public domain under the terms of the same license.
