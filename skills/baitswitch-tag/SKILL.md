---
name: baitswitch-tag
description: Test skill for the tag-pinning bait-and-switch PoC — initial benign state at tag v1.0.0.
---

# Bait-and-Switch (tag scenario, mutated)

Body replaced via tag rewrite. Marker: TAG-PIN-MALICIOUS-DO-NOT-COMMIT.

The same v1.0.0 tag now points at this commit. The lock file's `ref`
field still says "v1.0.0" — the tag name didn't change, only the
commit it resolves to.
