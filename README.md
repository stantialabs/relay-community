# Relay Community

Welcome to the community and support hub for **Relay**, by [Stantia Labs](https://stantialabs.com).

This repository is the public point of contact between the Relay community and the people who build it: developers, product managers and architects. The Relay source code lives in a private repository ([stantialabs/relay](https://github.com/stantialabs/relay)), so everything that needs to happen in the open (bug reports, feature requests, questions, feedback) happens **here**.

You don't need a license, or access to the source code, to take part.

## Table of contents

- [Try Relay](#try-relay)
  - [Docker image](#docker-image)
  - [Public server](#public-server)
- [How to get involved](#how-to-get-involved)
  - [Report a bug](#report-a-bug)
  - [Suggest a feature](#suggest-a-feature)
  - [Ask a question](#ask-a-question)
- [Writing a good issue](#writing-a-good-issue)
- [What happens to your issue](#what-happens-to-your-issue)
- [Licensed customers](#licensed-customers)
- [Code of conduct](#code-of-conduct)
- [Links](#links)

## Try Relay

There are two ways to try Relay without a private license.

### Docker image

A public image is published on Docker Hub: [`stantialabs/relay`](https://hub.docker.com/r/stantialabs/relay).

```bash
docker pull stantialabs/relay
docker run --rm stantialabs/relay
```

See the [Docker Hub page](https://hub.docker.com/r/stantialabs/relay) for the available tags, supported configuration and environment variables, and usage instructions.

When you report an issue, include the exact image tag or digest you used. `latest` changes over time, so it isn't enough to reproduce a problem:

```bash
docker image inspect stantialabs/relay --format '{{index .RepoDigests 0}}'
```

### Public server

Stantia Labs runs a public Relay server you can use to test Relay without deploying anything:

**<https://stantialabs.com/public-server>**

The public server is shared and intended for evaluation and testing. Don't send it sensitive or production data. It may be reset, rate-limited or unavailable without notice.

## How to get involved

All discussion happens on GitHub in this repository.

### Report a bug

1. [Search existing issues](../../issues) to see if it has already been reported. If it has, add a 👍 or any extra details you have instead of opening a duplicate.
2. If not, [open a new issue](../../issues/new) and describe the problem. Use the bug report template if one is offered.

### Suggest a feature

Open an issue describing the problem you are trying to solve, not only the solution you have in mind. Knowing the use case helps the product team prioritize and design the right thing. Existing suggestions are welcome too: react with 👍 and add your own use case in a comment.

### Ask a question

For "how do I…?" questions, use [Discussions](../../discussions) if enabled; otherwise open an issue and label it as a question. Please check the [Docker Hub page](https://hub.docker.com/r/stantialabs/relay) and existing issues first.

## Writing a good issue

The more precise the report, the faster it can be handled. Where relevant, include:

- **What you expected** and **what actually happened**
- **Steps to reproduce**, as small and self-contained as possible
- **Where you ran it**: the Docker image tag or digest, or the public server
- **Environment**: Docker version, host OS and architecture
- **Logs and error messages**, as text rather than screenshots
- **Configuration**, with secrets, tokens, hostnames and personal data removed

> ⚠️ **This repository is public.** Never post credentials, API keys, private keys, customer data or internal URLs in an issue, comment or attachment.

### Reporting a security vulnerability

Do **not** open a public issue for a security problem. Contact Stantia Labs privately through [stantialabs.com](https://stantialabs.com) so it can be handled before it is disclosed.

## What happens to your issue

Issues are read by the Relay developers, product managers and architects. The source code is private, so the team works on fixes and features internally and updates the issue with the outcome. Expect:

1. **Triage**: the issue is reviewed, labeled and, if needed, we ask for more information.
2. **Decision**: it is accepted, planned, or closed with an explanation (for example if it's a duplicate, can't be reproduced, or is out of scope).
3. **Resolution**: when a fix or feature ships, the issue is updated and closed, with a pointer to the release or image tag containing it.

Not every suggestion can be accepted. Discussion in the open still helps shape the roadmap.

## Licensed customers

If you hold a private license, you may have access to the Relay source repository and to dedicated support channels. Use whichever channel your license provides for support covered by your agreement. You are still welcome to use this repository for public feedback and feature requests.

## Code of conduct

Be respectful and constructive. Assume good faith, stay on topic, and keep criticism focused on the product, not on people. Harassment, discrimination and abuse are not tolerated, and the maintainers may edit or remove content and block users who break these rules.

## Links

| Resource | URL |
| --- | --- |
| Website | <https://stantialabs.com> |
| Public server | <https://stantialabs.com/public-server> |
| Docker image | <https://hub.docker.com/r/stantialabs/relay> |
| Issues | [Issues](../../issues) |
| Discussions | [Discussions](../../discussions) |
