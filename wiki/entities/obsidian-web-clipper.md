---
type: entity
name: "Obsidian Web Clipper"
kind: tool
aliases: ["Web Clipper"]
sources: [[llm-wiki-pattern-karpathy]]
tags: [tool, ingestion, obsidian]
---

# Obsidian Web Clipper

> Browser extension that converts web articles to markdown and drops them into an [[obsidian|Obsidian]] vault. Recommended in [[llm-wiki-pattern-karpathy]] as the primary on-ramp for getting web sources into the `raw/` layer of the [[llm-wiki-pattern]].

## Overview

Captures a web page, runs a readability pass, converts to markdown, and saves into a configured Obsidian vault folder. Pairs naturally with a hotkey ("Download attachments for current file") to also pull referenced images locally.

## Relationships

- Companion to [[obsidian]].
- Source of inputs for [[ingest-operation]].

## Mentioned in

- [[llm-wiki-pattern-karpathy]] — "Obsidian Web Clipper is a browser extension that converts web articles to markdown. Very useful for quickly getting sources into your raw collection."
