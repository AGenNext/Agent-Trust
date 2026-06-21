# agnxxt.com

Primary AGenNext platform domain.

## DNS records needed

```dns
@          A      51.161.208.75
www        CNAME  @
site       A      51.161.208.75
developers A      51.161.208.75
book       A      51.161.208.75
console    A      51.161.208.75
api        A      51.161.208.75
@          TXT    "agennext-domain=verified"
@          TXT    "agennext-owner=Chinmay Panda"
@          TXT    "agennext-github-org=AGenNext"
@          TXT    "agennext-trust-registry=https://github.com/AGenNext/Agent-Trust"
@          TXT    "v=spf1 -all"
_dmarc     TXT    "v=DMARC1; p=reject"
```

## Required files

- `.well-known/security.txt`
- `.well-known/did.json`
- `.well-known/agent-trust.json`
- `agennext.manifest.json`
- `autonomyx.manifest.json`
- `robots.txt`
- `sitemap.xml`
