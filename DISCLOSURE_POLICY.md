# Coordinated Disclosure Policy

This is how I handle vulnerabilities I discover in third-party software.

## Principles

- **Do no harm.** I test only what I am authorized to test, avoid accessing other users' data, and stop as soon as a vulnerability is proven.
- **Vendor first.** I report privately and give the vendor a fair chance to fix the issue.
- **Transparency after the fix.** Once users can protect themselves, I publish the details.

## Timeline (default)

| Day | Action |
|-----|--------|
| 0 | Private report sent to the vendor (security contact, bug bounty platform, or CNA) |
| 7 | If there is no acknowledgement, I send a second attempt through another channel |
| 90 | Default public disclosure deadline |
| +14 | Extension possible if a fix is ready and a release is imminent |

Exceptions: actively exploited vulnerabilities may be disclosed sooner; if the vendor is cooperative and needs more time, I will consider a reasonable extension in writing.

## Bug bounty programs

When a bounty or VDP is the reporting channel, **the program's rules override this policy** (including any non-disclosure clause). I publish nothing the program forbids.

## CVE assignment

I request CVE IDs through the vendor's CNA when one exists, otherwise through a CNA of last resort (e.g. MITRE) or the relevant ecosystem CNA.

## What an advisory contains

Affected versions, root cause, impact, CVSS, mitigation/fix, a proof of concept sufficient to verify the issue, a timeline, and credits. I avoid publishing weaponized exploit chains.
