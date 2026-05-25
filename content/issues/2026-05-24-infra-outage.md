---
title: Infrastructure provider outage
date: 2026-05-24 02:09:00
resolved: true
resolvedWhen: 2026-05-24 14:27:00
severity: down
section: issue
informational: false
pin: false

affected:
  - Build service
  - Website
  - API
  - Discourse
---

One of Flathub's infrastructure providers experienced an outage, which
caused multiple services to become unavailable. This issue has now been
resolved by the provider.

Any builds that were affected during the outage have been restarted.

- If a pull request test build is still failing, maintainers can
  restart it by commenting `bot, build` on the pull request.
- If an official build from a merged pull request is broken, please
  open an [issue](https://github.com/flathub/flathub/issues).

{{< track "2026-05-24 14:27:00" >}}
