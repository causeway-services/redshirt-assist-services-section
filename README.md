# Redshirt Assist Services Section

The app seat of Redshirt Assist at `https://redshirt-assist.561.group`, the
561 Group's Assist application for Target employees, beneath
public-worker-services-section. Founded 2026-09-11 in
the first prompt of the session that platformized
the Assist family: "We want to prepare for a new Assist application for our
web platform, for Target employees, at https://redshirt-assist.561.group."

## Not built as of 2026-09-11

Nothing of Redshirt Assist exists as code beyond this seat and its record.
This section exists so the app has a name, a data record, and a named
deploy shape before it is built.

## What it is

Redshirt Assist is one call of `createAssistWorker` from
[personal-intelligence-systems-services-section](../../../../../../../engineering-services-section/services/computer-engineering-services-section/services/computer-systems-engineering-services-section/services/personal-computer-systems-services-section/services/personal-intelligence-systems-services-section/README.md)
over the Assist application record at
`data/records/assist-application-service-record.json`, once its domain
section (the package that will supply its login adapter and tool registry)
exists. This seat carries no application logic of its own: everything
Redshirt Assist does is the engine, parameterized by its record, the same
way EVE Assist, Alpaca Assist, and Gig Assist each parameterize it.

## The deploy shape it will take

The same shape as the live precedent, eve-assist.561.group: a Cloudflare
Worker whose `wrangler.jsonc` binds a `public/` directory as static
assets, with `run_worker_first` for `/auth/*`, `/api/*`, and `/mcp`, a
custom-domain route, and a D1 database; `src/index.mjs` is a one-line
import of the engine's Worker handler. No application code is copied here.

## Open questions

- **Login provider.** Undecided: the Founder names the identity provider
  Target employees use.
- **Domain section.** Undecided: a retail-work domain section beside
  `personal-work-intelligence-systems-services-section` supplies the login
  adapter and tool registry.
- **Brand.** Undecided.

## Specification

See [The Assist application platform](../../../../../../../engineering-services-section/services/computer-engineering-services-section/services/computer-systems-engineering-services-section/services/personal-computer-systems-services-section/content/text/documents/articles/notes/2026/09/11/2026-09-11-assist-application-platform.md), the specification this
seat, EVE Assist, Alpaca Assist, and Gig Assist are each a parameterization
of.
