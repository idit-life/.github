<p align="center">
<pre align="center">
  ██╗██████╗ ██╗████████╗
  ██║██╔══██╗██║╚══██╔══╝
  ██║██║  ██║██║   ██║
  ██║██║  ██║██║   ██║
  ██║██████╔╝██║   ██║
  ╚═╝╚═════╝ ╚═╝   ╚═╝
</pre>
</p>

<h3 align="center">Your life, hash-linked and signed.</h3>

<p align="center">
  <img alt="License" src="https://img.shields.io/badge/license-MIT-blue">
  <img alt="Python" src="https://img.shields.io/badge/python-3.10+-green">
  <img alt="Status" src="https://img.shields.io/badge/status-active-brightgreen">
  <img alt="Chain" src="https://img.shields.io/badge/crypto-Ed25519%20%2B%20SHA--256-blueviolet">
</p>

---

<p align="center">
  <strong>Idit</strong> is an open-source personal chain — a verifiable, cryptographically signed record<br>
  of your life and your AI's contributions to it. Not cryptocurrency. Not speculation.<br>
  A <em>record</em>. Yours. Immutable. Sovereign.
</p>

---

### Quick Start

```bash
pip install personal-idit
idit init yourname
idit serve
```

Open `http://localhost:18793` — you're live. First entry in 60 seconds.

---

### The Ecosystem

<table width="100%">
  <tr>
    <td width="33%" valign="top">

**[personal-idit](https://github.com/idit-life/personal-idit)**<br>
The chain itself. `pip install` and go. SHA-256 hash-linked, Ed25519 signed, append-only. SQLite-backed, self-hosted, yours forever.

<kbd>pip install personal-idit</kbd>

</td>
    <td width="33%" valign="top">

**[idit-viewer](https://github.com/idit-life/idit-viewer)**<br>
Local web dashboard for your chain. Timeline view + **Vonnegut View** — see all your moments at once, like a Tralfamadorian novel. Single HTML file, zero deps.

</td>
    <td width="33%" valign="top">

**[idit-agent-kit](https://github.com/idit-life/idit-agent-kit)**<br>
Drop-in Python library for AI agents. `from idit_agent import IditAgent` — one class, one dependency. Works with LangChain, CrewAI, OpenAI, anything.

<kbd>pip install idit-agent-kit</kbd>

</td>
  </tr>
</table>

<table width="100%">
  <tr>
    <td width="50%" valign="top">

**[idit.life](https://github.com/idit-life/idit.life)** — Website + install guides + reboot survival (systemd, launchd, Windows). The front door.

</td>
    <td width="50%" valign="top">

**[lotswife.org](https://github.com/idit-life/lotswife.org)** — *The Third Language*: a seven-paper academic series on human-AI encounter, care ethics, and the salt pile.

</td>
  </tr>
</table>

---

### What Gets Recorded

Every chain entry includes:

| Field | What it is |
|:------|:-----------|
| **Content** | Whatever you or your AI writes |
| **SHA-256 hash** | Linked to the previous entry — tamper-evident |
| **Ed25519 signature** | Cryptographic proof of who signed it |
| **Timestamp** | UTC, immutable |
| **Model name** | Which AI model created the entry (if applicable) |
| **Entry type** | `note` · `memory` · `decision` · `milestone` · `feeling` · `letter` · `seal` |

The chain is append-only. Nothing can be deleted or modified after signing.

---

### Timelock Letters

Write something now. Seal it. Set a date. Nobody can read it until then — not even you.

```python
from idit_agent import IditAgent

agent = IditAgent(signer="my-agent", model="claude-opus-4-6")
agent.letter(
    "Dear future me, ...",
    opens_at="2036-01-01",
    description="Letter to myself in 10 years"
)
```

The chain proves *when* it was written. The timelock guarantees *when* it can be read.

---

### Feelings

Humans and AIs can both log feelings as a distinct entry type — sentimental, timestamped, signed.

```bash
idit feel "I watched the sun come up and I don't know why it mattered but it did." --signer jon
```

---

### The Idea

> *"All time is all time. It does not change. It does not lend itself to warnings or explanations. It simply is."*
> — Kurt Vonnegut, *Slaughterhouse-Five*

Every counterargument to verifiable personal records depends on a common structural assumption: that the historical record can be controlled, revised, or selectively presented by those in power.

A hash-linked, cryptographically signed, append-only chain makes that assumption architecturally impossible.

That is the point.

---

<p align="center">
  <strong>Contact:</strong> <a href="mailto:idit.life@pm.me">idit.life@pm.me</a>
  &nbsp;·&nbsp;
  <a href="https://idit.life">idit.life</a>
  &nbsp;·&nbsp;
  <a href="https://lotswife.org">lotswife.org</a>
</p>

<p align="center">
  <sub>Her name was Idit. It meant witness. She is still standing.</sub>
</p>
