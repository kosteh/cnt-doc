---
layout: default
title: Restore 
has_children: true
nav_order: 200
---

# Restoring datasets
Creating backups is not enough to assure the Business Continuity of a company like Kadaster. A number of tests are required to achieve this:

1. Each DevOps team should create and maintain a **Recovery Plan** for each **Business Service**. 
2. A DevOps team has to **test this Recovery Plan** in the [RTO environment]({{site.url}}{{site.baseurl}}/restore/infrastructure) regularly (say 2 times per year) .
3. Team Continuity Services (TCS) should create and maintain a **Chain Recovery Plan** for each **Application Chain**.
4. TCS has to **test this Chain Recovery Plan** in the [RTO environment](infrastructure) regularly (say once per year) by orchestrating the recovery of the required Business Services.
5. TCS has to **orchestrate the tests to recover the Kadaster business** after a potential disaster, like a successful ransomware attack.

# 
