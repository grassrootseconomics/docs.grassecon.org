# AGENTS.md

## Purpose and authority

This repository is the public Grassroots Economics documentation site. It owns organization-specific training, field methods, policies, legal source material, and historical software documentation. It is not the canonical source for current Cosmo-Local Credit (CLC) product or protocol behavior.

Use this authority order when sources differ:

1. The user's instructions.
2. `https://docs.cosmolocal.credit` for current CLC terminology, legal language, capability status, and whether a feature is current, deployment-dependent, historical, or proposed.
3. `https://cosmolocal.credit` for supported App behavior and routes.
4. This repository for Grassroots Economics training, policies, field practice, and archives.

Treat sibling repositories as read-only references unless the user explicitly expands the task.

## CLC migration rules

- Canonical App: `https://cosmolocal.credit`
- Canonical CLC documentation: `https://docs.cosmolocal.credit`
- Getting started: `https://docs.cosmolocal.credit/introduction/getting-started`
- History: `https://docs.cosmolocal.credit/introduction/history`
- Terms of Service: `https://docs.cosmolocal.credit/governance/terms`
- CLC source code: `https://github.com/cosmo-local-credit`
- Historical Sarafu dashboard: `https://dune.com/grassrootseconomics/sarafu-network`

Do not present Sarafu Network or `sarafu.network` as the current platform. The service formerly presented as Sarafu Network transitioned to CLC, but this does not imply that every historical account, wallet, token, voucher, Pool, balance, report, participant, or obligation migrated or remains available in the current App.

Sarafu may remain in publication titles, datasets, quotations, timelines, contract or component names, archived instructions, historical URLs, and legal source text. Mark surrounding material as historical, archived, or platform-specific so it cannot be mistaken for current CLC behavior. Do not substantively rewrite agreements, licenses, declarations, or other legal source text merely to replace the name; add a status notice and link to the current CLC Terms instead.

Keep current product claims conservative and sourceable. Distinguish between:

- capabilities available in the current CLC deployment;
- features dependent on a particular Pool, role, provider, configuration, or deployment;
- historical Sarafu activity; and
- proposed protocol or governance mechanisms.

Do not claim universal liquidity, automatic productive backing, guaranteed impact or redemption, permissionless App access, current USSD access, or guaranteed cash on/off-ramps without a current canonical source. Use broad governance language such as participants, issuers, Pool Stewards, cooperatives, public agencies, federations, multisigs, service providers, and other accountable structures. Do not introduce Regenerative Bonds branding unless explicitly requested.

## Editing approach

- Preserve the site's community-centered voice and keep changes concise and public-facing.
- Keep training and field materials on this site; point readers to the CLC docs for current App and protocol definitions.
- Prefer relative links for content that remains on `docs.grassecon.org`.
- Keep historical URLs, identifiers, screenshots, filenames, and source titles intact inside archived artifacts.
- `docs/` contains authored content, `mkdocs.yml` owns navigation and site configuration, and `overrides/` contains theme customizations.
- `public/` and `site/` are generated and ignored; never edit or commit them by hand.

## Validation

Install the pinned dependencies from `requirements.txt`, then run:

```bash
mkdocs build --strict
```

Also search tracked source for `sarafu`, `sarafu.network`, and `docs.grassecon.org`. Every remaining occurrence must be self-hosting configuration, an intentional organization-owned destination, or clearly marked historical, archival, or legal source material. Confirm that no page describes Sarafu Network as the current or live platform.
