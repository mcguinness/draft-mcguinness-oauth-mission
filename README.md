# Mission-Bound Authorization for OAuth 2.0

This is the working area for the individual Internet-Draft, "Mission-Bound
Authorization for OAuth 2.0".

* [Editor's Copy](https://mcguinness.github.io/draft-mcguinness-oauth-mission/#go.draft-mcguinness-oauth-mission.html)
* [Datatracker Page](https://datatracker.ietf.org/doc/draft-mcguinness-oauth-mission)
* [Individual Draft](https://datatracker.ietf.org/doc/html/draft-mcguinness-oauth-mission)
* [Compare Editor's Copy to Individual Draft](https://mcguinness.github.io/draft-mcguinness-oauth-mission/#go.draft-mcguinness-oauth-mission.diff)

## About

OAuth 2.0 issues access tokens for individual resource requests, but it has
no durable, approved artifact for the one task a user authorized an agent to
pursue. This document defines a **Mission**: a structured, human-approved,
integrity-bound OAuth authorization artifact. A client submits a Mission
Intent through PAR; the Authorization Server derives Rich Authorization
Requests authorization details, binds them to the approver's consent through
an integrity anchor, and records a durable Mission. Every derived access
token carries that authority and a `mission` claim, and issuance is gated on
the Mission's lifecycle state.

## Contributing

See the
[guidelines for contributions](https://github.com/mcguinness/draft-mcguinness-oauth-mission/blob/main/CONTRIBUTING.md).

Contributions can be made by creating pull requests.
The GitHub interface supports creating pull requests using the Edit (✏) button.

## Command Line Usage

Formatted text and HTML versions of the draft can be built using `make`.

```sh
$ make
```

Command line usage requires that you have the necessary software installed.
See [the instructions](https://github.com/martinthomson/i-d-template/blob/main/doc/SETUP.md).
