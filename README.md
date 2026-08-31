# Lago — Corresponding Source

This repository holds the **Corresponding Source** for the modified builds of
[Lago](https://github.com/getlago/lago) that Declara deploys, as required by the
GNU Affero General Public License v3.0, section 13.

There is no source code in this repository's history. Each
[release](../../releases) carries a `.tar.gz` containing the complete source of
one deployed version.

## What is in a release

Each tarball contains the superproject and both submodule trees — the API and the
front-end — plus a `DEPLOYED_VERSION` file naming the exact commits it was built
from:

```
version:      the deployed version
superproject: commit of this distribution
api:          commit of the modified lago-api
front:        commit of the unmodified lago-front
built_at:     when the tarball was produced
```

The tarball is produced by the same automated run that performs the deployment, so
it cannot drift from what is actually running.

## What was modified

The premium licence gates were removed from the API, and the AI assistant was
disabled. The front-end is unmodified. Each tarball contains `NOTICE.md` at its
root and `api/NOTICE.md`, which describe the changes in full.

## Licence

Lago is distributed under the GNU Affero General Public License v3.0. See
[`LICENSE`](LICENSE). This distribution is modified and is **not** an official
Lago release.

"Lago" and the Lago logo are trademarks of Getlago SAS. The AGPL grants no
trademark rights.
