---
type: entity
name: "Obsidian"
kind: product
aliases: []
sources: [[llm-wiki-pattern-karpathy]]
tags: [tool, markdown, obsidian]
---

# Obsidian

> Local-first markdown editor with `[[wikilinks]]`, plugin ecosystem, and a graph view. The wiki frontend for the [[llm-wiki-pattern|LLM Wiki pattern]] as described by [[andrej-karpathy|Karpathy]] — [[llm-wiki-pattern-karpathy]].

## Overview

Plain-text markdown editor that treats the vault as a folder of files on disk. Supports `[[wikilink]]` syntax, YAML frontmatter, a graph view of the link structure, and plugins like [[dataview]] and [[marp]].

## Notable work / output

- Native `[[wikilink]]` resolution across folders.
- Graph view — "the best way to see the shape of your wiki" per [[llm-wiki-pattern-karpathy]].
- Plugin ecosystem: [[dataview]], [[marp]], etc.
- Companion: [[obsidian-web-clipper]] browser extension.

## Relationships

- Pairs with [[claude-code]] (or any LLM agent) in the recommended workflow.
- Hosts the wiki layer of the [[llm-wiki-pattern]].
- Plugin: [[dataview]].
- Plugin: [[marp]].
- Companion extension: [[obsidian-web-clipper]].

## Mentioned in

- [[llm-wiki-pattern-karpathy]] — "Obsidian is the IDE; the LLM is the programmer; the wiki is the codebase."
