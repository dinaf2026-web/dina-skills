# dina-skills

A Claude Code plugin marketplace. It is a catalog, not a plugin. Nothing here
does any work: the file that matters is `.claude-plugin/marketplace.json`, which
points at the repositories where the skills actually live.

Add this one marketplace and every skill below becomes installable.

---

## Install

In Claude Code or Cowork: Settings, then Add marketplace, then paste this
repository's URL, then Sync.

Or from the command line:

```
/plugin marketplace add dinaf2026-web/dina-skills
/plugin install <plugin-name>@dina-skills
```

---

## What is in the catalog

| Plugin | What it does |
|---|---|
| [`business-audit-forensics`](https://github.com/dinaf2026-web/business-audit-forensics) | Business financial audit and forensic accounting. Two postures: internal audit of your own books, and adversarial investigation. Built around one rule, that a pattern is a hypothesis and not a finding until it is corroborated against a source document outside the ledger. Ships scripts for evidence custody, two-directional reconciliation, prior-year roll-forward, and an exception battery where every test carries a positive control. |
| [`ai-secure-code-review-guide`](https://github.com/dinaf2026-web/ai-secure-code-review-guide) | AI-led secure code review. Threat model, review, triage, report, plus a diff mode for pending changes. Language-agnostic core with a deep Android and Kotlin rule pack. An instruction guide, not a scanner. |

---

## Why the catalog is separate from the skills

Each skill lives in its own repository, with its own README, its own license and
its own history. Someone who only wants one of them can clone just that one.

This repository exists so they can be installed together from a single URL, and
so adding a third skill is a four-line change here rather than another
marketplace to add.

Entries are not pinned to a commit. Each one tracks its repository's default
branch, so a fix pushed to a skill reaches you without this catalog changing.

---

## License

The catalog itself is MIT, copyright 2026 Dina Farhat.

Each skill carries its own license and its own attribution notices. Check the
individual repository before reusing anything from it. `ai-secure-code-review-guide`
in particular is a derivative work and ships upstream license texts that are not
interchangeable with the canonical ones they resemble.
