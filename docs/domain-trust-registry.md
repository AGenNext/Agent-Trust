# AGenNext Domain Trust Registry

This registry connects known AGenNext, Autonomyx, OpenDataWorld, Unboxd Cloud, and related publication domains into one trust boundary.

The purpose is not only DNS routing. The purpose is authority binding.

A domain is treated as a trust surface only when ownership, publication, identity, policy, provenance, and security controls are explicitly verified.

## Operating Doctrine

```text
Domain
  ↓
Ownership Verification
  ↓
Identity Binding
  ↓
Policy Binding
  ↓
Publication Binding
  ↓
Agent Capability Binding
  ↓
Verification
```

No domain is trusted by name alone.

Every domain starts as untrusted until verified.

## Known Domains

| Domain | Owner / Org | Role | Status |
|---|---|---|---|
| `agnxxt.com` | AGenNext | Primary platform domain | Active known |
| `site.agnxxt.com` | AGenNext | Public site | Active known |
| `developers.agnxxt.com` | AGenNext | Developer portal | Active known |
| `book.agnxxt.com` | AGenNext | Book/docs surface | Active known |
| `console.agnxxt.com` | AGenNext | Console/admin surface | Active known |
| `openautonomyx.com` | openautonomyx | Autonomy/trust publication | Active known |
| `unboxd.cloud` | unboxd-cloud | Cloud/platform domain | Active known |
| `blog.unboxd.cloud` | unboxd-cloud | Blog/publication surface | Active known |
| `open-data.world` | OpenDataWorld | Data/fabric domain | Active known |
| `vps.open-data.world` | OpenDataWorld | VPS/server surface | Active known |
| `kubecontainer.xyz` | AGenNext | Kubecontainer experiment | Active known |
| `chinmay.sbs` | Personal author surface | Book/author publication | Active known |

## Required Domain Controls

Each production domain should expose:

```text
/.well-known/security.txt
/.well-known/did.json
/.well-known/agent-trust.json
/autonomyx.manifest.json
/agennext.manifest.json
/sitemap.xml
/robots.txt
```

Each production domain should also enforce:

- HTTPS/TLS
- canonical URLs
- security headers
- DNS ownership verification
- signed provenance manifest
- publication owner declaration
- no ambient agent authority

## Trust Policy

```yaml
default_state: untrusted_until_verified
browser_surface: governed
agent_surface: capability_bound
publication_surface: canonical_url_required
execution_surface: explicit_policy_required
```

## Binding Rule

A domain can publish content.

A domain can host applications.

A domain can expose APIs.

A domain can serve agents.

But a domain must not grant authority until it is bound to identity, policy, provenance, and verification.

## GitHub Organization Binding

The following GitHub orgs are part of the trust boundary inventory:

- AGenNext
- openautonomyx
- unboxd-cloud
- OpenDataWorld
- OpenSaaSApps
- opensaaslabs
- openagx
- autonomyxpro
- didoneworld
- TheFraudDatabase
- SovereignBharat
- open-lmx
- OpenFrameworks-World
- sovereignpbulishing
- fabric-db
- Verified-Services-Online

## Next Execution Step

Generate one `.well-known` trust bundle per domain:

```text
security.txt
did.json
agent-trust.json
autonomyx.manifest.json
agennext.manifest.json
```

Then each domain can be verified, routed, and governed independently while still belonging to the same trust graph.
