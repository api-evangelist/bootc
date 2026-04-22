# Bootc

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
