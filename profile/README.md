<p align="center">
  <img src="https://raw.githubusercontent.com/ForgeBYTES/.github/main/profile/logo.png" title="ForgeBYTES" alt="ForgeBYTES" width="600" />
</p>

---

## About ForgeBYTES

ForgeBYTES began as a hand-built ELF forensics engine and grew into an agentic analysis system. It does not chase signature feeds. It knows how a healthy Linux binary is shaped, from headers and segments to instruction flow, and treats every deviation as a fact worth explaining.

The engine trusts nothing a binary declares about itself. Every claim is verified against the bytes, every finding carries its mechanism and evidence, and the same input always produces the same report. Detection quality is measured continuously on a corpus of real malware and clean Linux binaries. The numbers on this page come straight from that ledger.

Humans read the forensic narrative. Agents connect over MCP and act on structured findings. Kurama, the built-in AI operator, drives the same commands a human would, so nothing it concludes is beyond audit.

## Why this design

Generative tooling has collapsed the cost of producing malware variants. Hashes and signatures are reactive by construction, so they arrive one sample too late, and a defense that waits for a feed will keep losing that race. Structure is harder to shed. A packer must still map executable pages, an implant must still arrange persistence, a flooder must still reach the network through syscalls. ForgeBYTES anchors detection in the invariants a binary needs in order to work, and those survive the churn of generated variants.

A static ruleset decays, so detection quality has to live in a loop. ForgeBYTES measures itself continuously against a corpus of real malware families and clean Linux binaries. Every false verdict becomes a tracked defect, a fix and a re-measurement, and the detectors evolve at the cadence of the threat rather than the cadence of a release cycle. The same class of automation that generates malware also hardens the engine. The rates published on this page are the output of that loop.

Agentic security systems need more than a verdict. An autonomous responder cannot plan its next action from the word suspicious. It needs the cause. Descriptive findings, each naming its mechanism and carrying the bytes that prove it, are composable primitives for that work. They are reproducible, comparable across samples and auditable after the fact. A score ends a conversation. A described deviation starts an investigation, and that is the input an agent can reason over.
