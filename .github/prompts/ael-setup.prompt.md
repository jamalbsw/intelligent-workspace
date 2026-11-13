---
description: Set up the AEL project in this repository
---

# AEL project setup

Prepare this repository for the requested AEL application without assuming that any application or desktop folders already exist.

## Before making changes

1. Inspect the repository, its instructions, existing files, and available toolchain. This repository may be empty; do not claim that setup is complete merely because files were created.
2. Confirm the intended application scope, runtime targets, and required build/test commands from available project materials. If they are not specified, ask the user before making structural or architectural choices.
3. Treat React 19 as the intended UI target.
4. Do not add the Nightingale dependency until the project owners confirm both a package version compatible with React 19 and access to the package feed. The currently available compatibility information lists React 16–18 only. Do not guess a version, attempt to work around missing feed permissions, or downgrade React to make the package install.
5. Use the [Nightingale Storybook](https://storybook.bswsites.com/?path=/docs/get-started-about-nightingale--page) as the current visual and documentation reference. Inspect the relevant foundation, component, pattern, and accessibility pages for each requested design.

## Implementation

- Make only the setup changes supported by confirmed requirements.
- Create directories and configuration files only when needed; never assume `app`, `desktop`, or component folders exist.
- Follow `AGENTS.md` and existing repository conventions. Keep configuration minimal and avoid adding unrelated scaffolding or dependencies.
- Until the official package is available, reference-mode previews may use native React, HTML, and CSS. Clearly label them as temporary approximations—not official Nightingale components—and do not claim their behavior or APIs match Nightingale.
- Keep the preview renderer behind an adapter boundary so it can later use the official package. Do not introduce a substitute component library.
- Before automating Storybook ingestion, verify that an officially supported machine-readable catalog is available; do not rely on undocumented endpoints.
- If the task requires actual Nightingale components rather than reference-mode previews, stop and report the outstanding compatibility or package-feed requirement.

## Completion

- Run the smallest relevant setup validation available, such as the configured type check, tests, or build. If the repository has no runnable validation yet, say so plainly.
- Summarize the files created or changed, validation results, and any unresolved prerequisite. Do not report unverified setup as complete.
