---
layout: newsletter
title: "OpenCATS July 2026 project update"
category: newsletter
permalink: /news/2026/july-project-update/
---

## July 2026 project update

It has been a busy few weeks for OpenCATS since the v0.10.0 release, with work continuing on usability, installation reliability, security hardening, and the foundations needed for future releases.

One of the most visible improvements is the addition of CAPTCHA validation for career portal applications. That should help reduce unwanted submissions while keeping the public application workflow available for teams that rely on the portal. Country support has also been added, giving OpenCATS a stronger base for international deployments and cleaner handling of location-related information.

There has also been a lot of work around installation and upgrades. The installer now does a better job of running existing-installation migrations before asking setup questions, and the site settings can prefill the phone country code during installation. Several schema and migration cleanups landed as well, including fixes for duplicate migration numbering, migration syntax, nullable definitions, and guarded migration keys. In short: less friction for fresh installs, and a more predictable path for maintained installations.

Security and data hygiene continued to receive attention. OpenCATS now denies direct Apache web access to the temporary directory, validates staged import file identifiers, and cleans up related records when entities are deleted. Those are the kind of behind-the-scenes changes that may not be flashy, but they help keep deployments safer and databases tidier over time.

The issue tracker was quieter for new reports during this period, with no new issues opened between the v0.10.0 release and this update. A few older issues were closed, including reports about phone field validation, missing field definition IDs for required address fields, and activity logging offering jobs that should not appear. Another longer-running discussion about activity stream sorting and pagination was updated and remains open, so it is still available for anyone interested in improving how activity history is reviewed.

Developers and contributors should also notice ongoing modernization. The project has continued moving toward stronger PHP 8 compatibility, replacing legacy database result handling, removing old licensing code, and improving test coverage and CI reporting. Behat screenshots and JUnit reports are now easier to review from CI, Dependabot automation has been improved, and dependency updates are continuing to flow through the project.

We plan to continue publishing these project summaries monthly so the community can follow what changed, what was fixed, and which issues still need attention without having to read every commit or pull request individually. As always, if you are testing OpenCATS or running it in production, please keep sharing feedback through the project's GitHub issue tracker and discussions. The recent work is a good reminder that OpenCATS is improving not just through big releases, but through steady maintenance, review, and community contributions.
