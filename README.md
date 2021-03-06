# implementation decisions

A repository for all concrete decisions made about how to implement the
cardano blockchain. This repository contains all the technical details
and improvements that is needed for the developers.

Regarding the formal specifications, the repository contains a git submodule
that pin down a specific version of the formal specifications. Changes to
this need to be reflected in the different documents.

The "RFC" (request for comments) process is intended to provide a consistent
and controlled path for new features to enter the blockchain and standard
APIs, so that all stakeholders can be confident about the direction the
blockchain is evolving in.

# When to write a proposal

Currently we only accept proposals and comments from within the IOHK
organization.

Proposals are to be made if:

1. the formal specification is too vague and a concrete decision needs to be
   taken. Example: it is said the we take an index `idx` from the set of `Idx`.
   However there is not specification wether it is acceptable to have negative
   indices or if it is bounded (32bits? 64bits?), of if it is from 0 or from 1.
   A proposal can be made to pin this down and guarantee that we are all talking
   about the same thing.
2. the current blockchain needs to include new features in order to implement the
   new feature defined by the formal spec. This needs to be documented here too.
3. an improvement to the current implementation needs to be made. For example
   one could propose an improvement to the way we serialize blocks.

# The process

1. fork this repository;
2. Copy 0000-template.md to text/0000-my-feature.md (where "my-feature" is descriptive. don't assign an RFC number yet).
3. Fill in the RFC;
4. Submit a pull request. As a pull request the RFC will receive design feedback, and the author should be prepared to revise it in response
5. The owners of this repository will orchestrate the review process. They will follow
   the comments and will direct the conversation toward consensus. If no consensus can
   be reach in a timely manner they may: close the PR or apply any changes they believe
   to be necessary before merging the PR.

# License

This repository is currently in the process of being licensed under either of

Apache License, Version 2.0, (LICENSE-APACHE or http://www.apache.org/licenses/LICENSE-2.0)
MIT license (LICENSE-MIT or http://opensource.org/licenses/MIT)
at your option.

# Contributions

Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without any additional terms or conditions.
