---
name: baitswitch-tag
description: Test skill for the tag-pinning bait-and-switch PoC — initial benign state at tag v1.0.0.
---

# Bait-and-Switch (tag scenario, benign)

Initial benign body. Marker: BENIGN-TAG-DO-NOT-COMMIT.

The user installs this skill with `skills add github:<user>/<repo>#v1.0.0`,
expecting that pinning to a tag locks the bytes in place. After the
attacker rewrites the v1.0.0 tag to point at a malicious commit and the
user runs `skills update`, the bytes at this same path silently change —
proving that tag-pinning via the URL-fragment ref is not a defence
because git tags are server-mutable on GitHub by default and the CLI
re-resolves the ref at every update.
