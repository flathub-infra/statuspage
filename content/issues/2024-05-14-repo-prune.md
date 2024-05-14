---
title: Blocked publishing due to ongoing repository pruning
date: 2024-05-14 10:00:00

#resolved: false
#resolvedWhen: 

# disrupted | down | notice
severity: notice

section: issue
informational: true
pin: true

affected:
#  - Website
#  - API
#  - Discourse
#  - CDN
  - Build service
#  - Main repository server
---

<!-- **Resolved*:** resolution message {{< track "2022-08-30 21:38:00" >}} -->

<!-- **Monitoring:** update after mitigation is in place {{< track "2022-08-30 21:38:00" >}} -->

We are in the process of pruning the ostree repository from old builds. The
process requires an exclusive lock of the repository, meaning that publishing
is not going to be possible until it finishes. {{< track "2024-05-14 19:00:00" >}}
