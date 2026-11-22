<p align="center">
  <img src="harpe-banner.png" alt="Harpe Labs — Every defense has a hook." width="100%">
</p>

<p align="center">
  <strong>An independent security research collective.</strong><br>
  Web3 · AI · Applied offensive research
</p>

<p align="center">
  <a href="#open-for-audit"><img src="https://img.shields.io/badge/status-open%20for%20audit-F2EFE6?style=flat-square&labelColor=0A0A0A" alt="Open for audit"></a>
  <a href="#where-we-work"><img src="https://img.shields.io/badge/focus-web3%20%7C%20AI%20security-F2EFE6?style=flat-square&labelColor=0A0A0A" alt="Focus"></a>
</p>

---
# Harpe Labs

**We find the assumption your system is quietly relying on, then break it before someone else does.**

Somewhere in your codebase, someone wrote "this can never happen" and moved on. We go looking for that line. 
That's the hook.
We're a crew of independent security researchers, and finding that assumption is the whole job.

We are not a compliance shop. You won't get a checklist and a printout of scanner output from us. We assume your system was built by capable people, which means the way in is somewhere nobody thought to look. That's where we spend our time.

## Why "Harpe"

The harpe is the hooked sword Perseus carried against Medusa, a monster you can't look at head-on. The hook catches the shield and drags the defense out of position, and then the blade does its work. In our world, the hook is the assumption. We don't charge hardened surfaces. We find the hook.

**Every defense has one.**

## What we do

| Domain | Scope | The assumption we go after |
|---|---|---|
| **Smart contract security** | EVM / Solidity, Solana / Anchor, Move (Sui, Aptos), TRON. Protocol logic, economic and MEV attack paths, upgrade and access-control flaws, cross-chain and bridge assumptions. | "This invariant holds." It does, in every test, until someone orders the transactions differently. |
| **AI / ML security** | Prompt injection and tool-call abuse, agent and RAG pipeline compromise, model supply chain, data exfiltration through inference, guardrail bypass in production LLM systems. | "The agent will use its tools the way we pictured." Especially the agents that hold keys, funds or user data. |
| **Web & API** | Authentication and authorization logic, business-logic abuse, server-side request forgery, chained low-severity findings that compose into critical ones. | "Nobody would send that request." Somebody always does. |
| **Infrastructure review** | Key management, signer and multisig process, deployment pipelines, the operational gaps between a secure contract and an insecure org. | "The contract is audited, so we're safe." Not if the signer setup is a mess. |

## Receipts

Our researchers build the tools they wish they had during engagements. Some of them have been noticed.

### Tools in Pashov's AI Web3 Security Tools Hub

Two of our tools are listed in [Pashov's AI Web3 Security Tools Hub](https://github.com/pashov/ai-web3-security).

- **[Chase](https://github.com/0xCyrildev/Chase)** (Sui Move): open-source dynamic analysis of executed Sui Move transactions. Ships as a CLI, a library and an MCP server, and runs 8 invariant checks.
- **[Dot](https://github.com/0xCyrildev/dot)** (Solana): agentic blast-radius analysis for Solana program upgrades, built from CPI traces rather than source code.

### BountyForge

**[BountyForge](https://bountyforge.xyz/)** is an autonomous pentesting platform built by our researcher [Gabson0x](https://github.com/Gabson0x). It plans its own attacks, runs them in isolated sandboxes, and only reports a finding if it survives a replay against the live target, with a PoC and a CVSS score attached. It covers web, APIs and smart contracts (Solidity, Solana, Move). The site reports 22 hunting agents, 90 security tools, 9 validation gates and 1,000+ vulnerabilities spotted across live hunts on public programs.

More coming as we publish.

## Our aim

To make exploitation uneconomical for the systems we work on. We find the issue first, prove it with a working path, and stay until it's fixed instead of just filed.

## Our objectives

- **Proof over speculation.** Every finding ships with a reproduction. If we can't demonstrate it, we don't claim it.
- **Impact over volume.** One critical with a clear exploit path beats forty informational notes. We don't pad reports.
- **Fixes, not just findings.** A finding closes when the remediation is verified, not when the report is sent.
- **Research that outlives the engagement.** Once disclosure is complete, novel findings become public writeups and tooling, so the next team doesn't rediscover them from scratch.
- **Show up early on new surfaces.** AI systems are being shipped faster than they're being secured. We put research time there before the demand arrives.

## Where we work

We're active across public and private programs on **HackerOne**, **Bugcrowd**, **Immunefi**, **Intigriti**, **HackenProof** and **Cantina**, alongside direct client engagements.

## Open for audit

We're currently **taking engagements**. We're a good fit if you are:

- shipping a new contract system or a major upgrade
- deploying LLM agents with real tool access, funds or user data
- already audited and wanting an adversarial second pass
- pre-launch and wanting a researcher in the room before the code freezes, not after

**What an engagement looks like**

1. **Scope.** We review the codebase, the threat model and what the system is actually protecting. You get a flat quote and a timeline before any money moves.
2. **Research.** Manual review first, tooling second. We test the system against its own assumptions.
3. **Report.** Findings with severity, reproduction steps, impact analysis and concrete remediation.
4. **Verification.** We re-test every fix. No finding closes on your word or ours alone.

## Get in touch

| | |
|---|---|
| Audit inquiries | [YOUR EMAIL] |
| Security disclosures | [YOUR SECURITY EMAIL] |
| X / Twitter | [@harpelabs](https://x.com/harpelabs) |
| Telegram | [YOUR HANDLE] |

> If you are reporting a vulnerability in something we maintain, email the disclosure address above. We respond within 48 hours and we do not pursue researchers acting in good faith.

---

<p align="center">
  <sub><strong>HARPE LABS</strong> · Every defense has a hook.</sub>
</p>
