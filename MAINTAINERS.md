# Maintainers

This file defines the Maintainers processes (adding, removing) and duties for all repositories in the Hyperledger Aries Project,
as well as the list of Maintainers for this repository. "Maintainers" are defined as any individuals with escalated GitHub privileges above
"READ" in Hyperledger Aries repositories. Maintainers **MUST** abide by the Hyperledger Aries Project Charter.

All other Hyperledger Aries Project repository MAINTAINERS.md files point to this file.

## Maintainers for this Repository

Maintainers for this repository are listed in the [Access Control YAML file].
Search in the file for this repository.

[Access Control YAML file]: https://github.com/hyperledger/governance/blob/main/access-control.yaml

## The Duties of a Maintainer

Maintainers are expected to fulfill the following responsibilities for the repositories they oversee. The duties are listed in more or less priority order:

- Review, respond, and act on any security vulnerabilities reported against the repository.
- Review, provide feedback on, and merge or reject GitHub Pull Requests from
  Contributors.
- Review, triage, comment on, and close GitHub Issues
  submitted by Contributors.
- When appropriate, lead/facilitate architectural discussions in the community.
- When appropriate, lead/facilitate the creation of a product roadmap.
- Create, clarify, and label issues to be worked on by Contributors.
- Ensure that there is a well defined (and ideally automated) product test and
  release pipeline, including the publication of release artifacts.
- When appropriate, execute the product release process.
- Maintain the repository CONTRIBUTING.md file and getting started documents to
  give guidance and encouragement to those wanting to contribute to the product, and those wanting to become maintainers.
- Contribute to the product via GitHub Pull Requests.
- Monitor requests from the Hyperledger Technical Oversight Committee about the
contents and management of Hyperledger repositories, such as branch handling,
required files in repositories and so on.
- Contribute to the Hyperledger Project's Quarterly Report.

## Becoming a Maintainer

This community welcomes contributions. Interested contributors are encouraged to
progress to become maintainers. To become a maintainer the following steps
occur, roughly in order.

- The proposed maintainer establishes their reputation in the community,
  including authoring five (5) significant merged pull requests, and expresses
  an interest in becoming a maintainer for the repository.
- A PR is created to update the [Access Control YAML file] to add the proposed maintainer on team with appropriate privileges in the relevant repositories.
- The PR is authored by an existing maintainer or has a comment on the PR from an existing maintainer supporting the proposal.
- The PR is authored by the proposed maintainer or has a comment on the PR from the proposed maintainer confirming their interest in being a maintainer.
  - The PR or comment from the proposed maintainer must include their
    willingness to be a long-term (more than 6 month) maintainer.
- Once the PR and necessary comments have been received, an approval timeframe begins.
- The PR **MUST** be communicated on all appropriate communication channels, including relevant community calls, chat channels and mailing lists. Comments of support from the community are welcome.
- The PR is merged and the proposed maintainer becomes a maintainer if either:
  - At least three (3) TSC or project Maintainers approve the PR or provide an approval comment on the PR.
- If the PR does not get the requisite PR approvals, it may be closed.

## Removing Maintainers

Being a maintainer is not a status symbol or a title to be carried
indefinitely. It will occasionally be necessary and appropriate to move a
maintainer to emeritus status. This can occur in the following situations:

- Resignation of a maintainer.
- Violation of the Code of Conduct warranting removal.
- Inactivity.
  - A general measure of inactivity will be no commits or code review comments
    for one reporting quarter. This will not be strictly enforced if
    the maintainer expresses a reasonable intent to continue contributing.
  - Reasonable exceptions to inactivity will be granted for known long term
    leave such as parental leave and medical leave.
- Other circumstances at the discretion of the other Maintainers.

The process to remove a maintainer from active status is comparable to the process for adding a maintainer, outlined above. In the case of voluntary
resignation, the Pull Request can be merged following a maintainer PR approval. If the removal is for any other reason, the following steps **SHOULD** be followed:

- A PR is created to update the [Access Control YAML file] to remove the maintainer from the appropriate teams.
- The PR is authored by, or has a comment supporting the proposal from, an existing maintainer or Hyperledger GitHub organization administrator.
- Once the PR and necessary comments have been received, the approval timeframe begins.
- The PR **MAY** be communicated on appropriate communication channels, including relevant community calls, chat channels and mailing lists.
- The PR is merged and the maintainer is removed if:
  - The PR is approved by the maintainer to be removed, OR
  - At least three (3) TSC or Aries Project maintainer PR approvals or approval comments have been recorded.
- If the PR does not get the requisite PR approvals, it may be closed.

Returning to active maintainer status after being removed uses the same steps as adding a
new maintainer. Note that the emeritus maintainer already has the 5 required
significant changes as there is no contribution time horizon for those.
