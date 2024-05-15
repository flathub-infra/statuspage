---
title: Blocked publishing due to ongoing repository pruning
date: 2024-05-14 10:00:00

#resolved: false
#resolvedWhen: 

# disrupted | down | notice
severity: disrupted

section: issue
informational: false
pin: false

affected:
  - Build service
  - Main repository server
#  - Website
#  - API
#  - Discourse
#  - CDN
---

<!-- **Resolved*:** resolution message {{< track "2022-08-30 21:38:00" >}} -->

<!-- **Monitoring:** update after mitigation is in place {{< track "2022-08-30 21:38:00" >}} -->

The pruning process is still ongoing. It may take about 12 hours more. {{< track "2024-05-14 05:30:00" >}}

We are in the process of pruning the ostree repository from old builds. The
process requires an exclusive lock of the repository, meaning that publishing
is not going to be possible until it finishes. We will manually publish the
outstanding builds afterwards. {{< track "2024-05-14 19:00:00" >}}
