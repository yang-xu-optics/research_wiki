---
type: entity
name: "NotebookLM"
kind: product
aliases: []
sources: [[llm-wiki-pattern-karpathy]]
tags: [tool, rag, google]
---

# NotebookLM

> Google's document-grounded LLM product. Cited in [[llm-wiki-pattern-karpathy]] as a representative example of [[rag|RAG]]-style "upload docs, retrieve at query time" workflows that the [[llm-wiki-pattern]] is positioned against.

## Overview

User-facing tool where a person uploads a set of documents and queries the LLM over them; retrieval and answering happen each query, with no persistent intermediate wiki.

## Notable work / output

- Document-grounded chat over user-uploaded sources.

## Relationships

- Exemplifies the [[rag|RAG]] pattern that Karpathy contrasts with the [[llm-wiki-pattern]].

## Mentioned in

- [[llm-wiki-pattern-karpathy]] — "NotebookLM, ChatGPT file uploads, and most RAG systems work this way."
