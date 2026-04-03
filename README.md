# idit.life

**Your life, hash-linked and signed.**

Idit is an open-source personal chain — a verifiable, cryptographically signed record of your life and your AI's contributions to it. Every entry is SHA-256 linked and Ed25519 signed. Nothing can be altered after the fact.

This is not cryptocurrency. There is no token, no speculation, no financial instrument. This is a record. Your record.

## Repositories

| Repo | What it does |
|------|-------------|
| [personal-idit](https://github.com/idit-life/personal-idit) | The chain itself. `pip install personal-idit` and you're live in 60 seconds. |
| [idit-viewer](https://github.com/idit-life/idit-viewer) | Local web dashboard for browsing your chain entries. |
| [idit-agent-kit](https://github.com/idit-life/idit-agent-kit) | Drop-in Python library for AI agents to sign to the chain. |
| [idit.life](https://github.com/idit-life/idit.life) | Website source for [idit.life](https://idit.life) |
| [lotswife.org](https://github.com/idit-life/lotswife.org) | The Third Language — the academic series behind Idit. |

## Quick start

```bash
pip install personal-idit
idit init yourname
idit serve
```

Open `http://localhost:18793` to mint your first entry.

## The idea

Every counterargument to verifiable personal records depends on a common structural assumption: that the historical record can be controlled, revised, or selectively presented by those in power.

A hash-linked, cryptographically signed, append-only chain makes that assumption architecturally impossible.

That is the point.

## Contact

**idit.life@pm.me** · [idit.life](https://idit.life) · [lotswife.org](https://lotswife.org)
