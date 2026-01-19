# Web Server (C / C++)

> This repository is a fork of an existing project.
> I worked on this fork independently as part of my learning and experimentation.
> The sections below describe **my personal contributions** and how I used **AI coding tools** during development.

---

## What I built

A custom HTTP web server implemented in C/C++ using low-level system APIs.
The server supports configuration-based behavior and multiple production-style features such as CGI execution, redirects, and autoindexing.

This project was treated as a real backend system rather than an academic exercise.

---

## My Contributions

In my fork, I implemented and worked on the following features:

- Configuration file parsing inspired by Nginx-style configs.
- CGI execution for dynamic content handling.
- HTTP redirects and route-level configuration.
- Autoindex support for directory listing.
- Concurrent client handling using a poll-based I/O model.
- Error handling, edge cases, and robustness improvements.

---

## Why I built it

I wanted to deeply understand how real web servers work under the hood:
- sockets and network programming
- concurrency and I/O multiplexing
- HTTP behavior and edge cases
- process management (CGI)

I also wanted a realistic environment to experiment with **AI-assisted coding** on non-trivial, low-level systems code.

---

## How I used AI Coding Tools

I used AI coding tools (GitHub Copilot Chat, Cursor) as a **pair programmer**, not as an automatic code generator.

Specifically, I used AI for:
- Discussing design trade-offs for config parsing and CGI execution.
- Exploring alternative approaches to HTTP routing and redirects.
- Reviewing parsing logic for edge cases and malformed input.
- Refactoring code for readability and maintainability.
- Clarifying low-level APIs and system behavior during debugging.

All architectural decisions and final implementations were validated and controlled manually.

---

## Where AI helped

- Identifying edge cases in HTTP request parsing.
- Suggesting cleaner abstractions for configuration handling.
- Speeding up iteration during refactoring.
- Acting as a second reviewer when reasoning about complex control flow.

---

## Where AI was wrong

- Suggested unsafe memory ownership patterns for config parsing.
- Proposed blocking I/O approaches that did not scale well.
- Missed edge cases in CGI process cleanup and error handling.
- Over-simplified HTTP behavior that required manual correction.

This forced me to critically evaluate AI output instead of blindly accepting it.

---

## My AI Coding Workflow

1. Start with my own design and mental model.
2. Use AI to challenge assumptions or explore alternatives.
3. Implement solutions manually.
4. Use AI again for review and edge-case discussion.
5. Test aggressively and fix failure modes.

I treat AI as a productivity multiplier, not as a source of truth.

---

## Using myself as first customer

I tested the server by:
- Writing multiple configuration variants.
- Running malformed and edge-case HTTP requests.
- Stress-testing concurrent connections.
- Observing failure modes and improving error handling.

I approached the project as if I were a real user of the system.

---

## What I learned

- How to integrate AI coding tools into real systems programming.
- Where AI accelerates development — and where it becomes dangerous.
- How to maintain architectural ownership while using AI.
- How low-level systems code benefits from careful, critical AI usage.

---

## Why this project fits the AI Vibe Coder role

This project demonstrates:
- Bias to action — I built and extended a real system.
- Problem awareness — I identified and fixed real-world edge cases.
- Obsession to learn — I used AI to deepen my understanding, not replace it.
- Product thinking — I treated the server as a usable product.
- Engineering judgment — I accepted, rejected, and corrected AI suggestions.

---

If helpful, I’m happy to walk through the code, decisions, and AI workflow in more detail.
