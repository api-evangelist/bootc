# Bootc

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Bootc is an open source tool that enables transactional, in-place operating system updates using OCI/Docker container images as the source for OS updates. It applies the container layering model to bootable host systems, using standard OCI containers as a transport and delivery format for base OS updates. The container image includes a Linux kernel, and when deployed the base userspace runs normally with systemd as PID 1. Bootc is a CNCF Sandbox project with a stable CLI and API.

**URL:** [https://bootc.dev](https://bootc.dev)

**Documentation:** [https://bootc.dev/bootc/](https://bootc.dev/bootc/)

**GitHub:** [https://github.com/bootc-dev/bootc](https://github.com/bootc-dev/bootc)

**APIs.yml:** [View APIs Index](https://raw.githubusercontent.com/api-evangelist/bootc/refs/heads/main/apis.yml)

## CLI Commands

| Command | Description |
|---------|-------------|
| `bootc upgrade` | Pull the latest OCI image and stage a new deployment |
| `bootc upgrade --apply` | Upgrade and auto-apply on next reboot |
| `bootc upgrade --download-only` | Download update without applying |
| `bootc switch <image>` | Change the container image reference being tracked |
| `bootc status` | Display current booted image and staged changes |
| `bootc rollback` | Revert to previous boot entry |
| `bootc install to-disk` | Install OS image to a disk |
| `bootc install to-filesystem` | Install OS image to a filesystem |

## Use Cases

- Transactional OS updates using container images
- Immutable/reproducible infrastructure
- GitOps-style OS management
- Air-gapped and offline OS deployments
- Container-native operating system delivery

## Community

- CNCF Slack: #bootc-dev
- Weekly meetings: Fridays at 15:30 UTC on CNCF Zoom

## Maintainers

- **Kin Lane** - kinlane@gmail.com
