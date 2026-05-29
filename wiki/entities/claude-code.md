---
type: entity
name: "Claude Code"
kind: product
aliases: []
sources: [[llm-wiki-pattern-karpathy]]
tags: [tool, llm-agent, anthropic]
---

# Claude Code

> Anthropic's coding-agent CLI. Reads a `CLAUDE.md` file in the working directory as its schema/instructions — which is the mechanism by which the [[llm-wiki-pattern|LLM Wiki pattern]] in this vault is implemented.

## Overview

LLM agent shipped by Anthropic that operates over a local filesystem. Looks for `CLAUDE.md` to learn project-specific conventions. In this vault, `CLAUDE.md` *is* the schema layer of the [[llm-wiki-pattern]].

## Notable work / output

- Reads `CLAUDE.md` to load per-project schema/instructions.
- Comparable role to Codex's `AGENTS.md`, OpenCode's project config, etc.

## Relationships

- Authored by Anthropic.
- Named alongside Codex, OpenCode, Pi in [[llm-wiki-pattern-karpathy]] as agents the pattern can run on.
- Pairs with [[obsidian]] as frontend.

## Mentioned in

- [[llm-wiki-pattern-karpathy]] — listed as an example agent the gist is intended to be shared with.
