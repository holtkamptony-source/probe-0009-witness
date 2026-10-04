# probe-0009-witness

Timestamp witness for the PROBE-0009 pre-registration, a designed tier
benchmark of the KV-AUDIT paper-audit plugin. PROBE-0009 succeeds
PROBE-0008, whose witness is `probe-0008-witness`, and PROBE-0007, whose
witness is `probe-0007-witness`. The three are never mixed.

## What this repository is for

Before a chosen arXiv announcement, the probe's executor pushes one small
precommitment file here. GitHub's server-side push event for that push,
read from the public Events API, is the timestamp receipt: it shows the
file existed before the announcement. A Git author or committer date is
never used as the receipt, because anyone can set it.

## What it holds

Each precommitment file holds only:

- the intended announcement instant and the date the listing will state;
- a commitment to the draw seed (a sha256);
- the sha256 of the probe's exclusion inventory;
- the pre-registration's canonical hash.

## What it never holds

No pilot evidence, no paper text, no reads, no results, and nothing else
from the project.

## Limits

There is no independent custodian. A receipt could be withheld, or a
pushed reference deleted, without this repository alone revealing it.
The pre-registration states this limitation.
