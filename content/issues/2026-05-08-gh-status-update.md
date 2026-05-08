---
title: Build status updates failing
date: 2026-05-07 16:03:00
resolved: true
resolvedWhen: 2026-05-08 10:50:00

# disrupted | down | notice
severity: disrupted

section: issue
informational: false
pin: false

affected:
  - Build service
#  - Main repository server
#  - Website
#  - API
#  - Discourse
#  - CDN
---

GitHub pull request status updates, branch commit statuses, and
flathubbot comments were failing due to a missing token in the
build service configuration, despite builds being completed
successfully. As a result, affected pull requests did not receive
status updates or completion comments, and branch commit statuses were
not being updated.

The issue has been resolved now, and all affected open pull requests
should be updated with their build statuses. Some commit statuses may
still remain outdated, but this does not affect the publishing
process.

If any pull request completed successfully but still lacks a status
update, please restart the build by commenting `bot, build` on the pull
request. {{< track "2026-05-08 10:50:00" >}}
