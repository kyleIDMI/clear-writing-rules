# Clear Writing Rules

A portable Agent Skill that makes an AI agent write clearly, accurately, and like a human. It is general-purpose: emails, customer notes, internal memos, documentation, status updates, anything made of sentences. It is not tied to any wiki, CMS, or publishing system.

Compatible with Claude Code, OpenAI Codex, Cursor, Windsurf, and agents that follow the [Agent Skills specification](https://agentskills.io/specification.md).

## Why this exists

Unedited AI output has tells: em dashes everywhere, words like "leverage" and "furthermore", openers like "in today's world", hollow sentences that assert importance without a fact, and a uniform structure that reads like a template. The bigger risk in business writing is accuracy: a model will produce a confident-sounding number, date, or quote that is simply wrong.

This skill addresses both. It strips those patterns and it enforces that every fact, figure, and attribution is real. It does not touch your tone. A payment notice, a goodwill apology, and a claims update each need a different register, and that judgment stays with the writer.

## What it does

When you ask an agent to write or edit prose, it reads the skill, writes against the rules, then self-checks the output against a banned-words and patterns reference before returning it. The rules cover:

- **Accuracy:** no fabricated numbers, dates, quotes, attributions, case studies, or history.
- **Vocabulary:** no AI verbs (delve, leverage, utilize), no AI transitions (furthermore, moreover), no academic tells (a myriad of, paramount).
- **Phrasing:** no filler openers, no hollow statements, no weasel words, no em dashes.
- **Structure:** vary paragraph and sentence length so it does not read like a machine template.

Tone-related rules are scoped to ban manufactured hype, not genuine warmth.

## Appropriate use

This is a writing-quality and accuracy aid. It is not a tool for disguising AI authorship or defeating AI detectors. Follow your organization's policy on AI use and disclosure. The goal is to read your own draft, ground it in real facts, and make it sound like a person wrote it before your name goes on it.

## Who it is for

Anyone at the company who drafts written communication with an AI assistant: support and customer-facing staff, project managers, finance, HR, and management. The accuracy guardrails matter most where a wrong detail has consequences.

## Installation

### Desktop or web app (claude.ai)

1. Enable the prerequisite: in Claude, go to **Settings > Capabilities** and turn on **Code execution and file creation**.
2. Download the skill ZIP: [clear-writing.zip](https://github.com/kyleIDMI/clear-writing-rules/releases/latest/download/clear-writing.zip) (always the latest release).
3. Go to **Customize > Skills**, click **+**, choose **Create skill**, and upload the ZIP.
4. It appears under **Personal skills**. Toggle it on.

An admin can upload the same ZIP as an organization skill to make it available to everyone automatically.

### Claude Code plugin

```bash
/plugin marketplace add kyleIDMI/clear-writing-rules
/plugin install clear-writing-rules
```

You can also read the files yourself as a style guide. Every file here obeys its own rules, so they double as worked examples.

## What each file does

| File | Contents |
|---|---|
| `CLAUDE.md` | Claude Code entrypoint. States the purpose, what the package enforces versus what it leaves alone, the operating rules, and all 24 rules. |
| `AGENTS.md` | Cross-agent repository instructions and format notes. |
| `.claude-plugin/marketplace.json` | Claude Code plugin marketplace manifest. |
| `skills/clear-writing/SKILL.md` | The rules as actionable guidance, with WRONG/RIGHT worked examples and a self-check pass. |
| `skills/clear-writing/references/ai-writing-detection.md` | The full banned-words reference: verbs, adjectives, transitions, phrases, intensifiers, heading anti-patterns, academic tells, hedging markers, and structural and statistical patterns. |
| `.claude/skills/` | Claude Code project-local mirror of the published skill. |

## Credit

Adapted from [realrossmanngroup/no_ai_slop_writing_rules](https://github.com/realrossmanngroup/no_ai_slop_writing_rules). This fork removes the Louis Rossmann voice profile and reframes the package as a tone-neutral writing-quality aid for business communication. The anti-slop rules and the writing-detection reference are derived from that project.
