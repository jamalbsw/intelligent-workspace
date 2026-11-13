# Repository guidance

## Starting work

- Inspect the repository and its current documentation before making changes. Do not assume application, desktop, or component folders exist.
- Keep changes focused on the requested task. Preserve established conventions where they exist; when the repository is still a blank slate, document important choices in the relevant project documentation.
- Do not add dependencies, credentials, or environment-specific configuration without a clear need. Never commit secrets.
- Run the smallest relevant validation available and report what was run and any blockers.

## UI framework and component library

- React 19 is the intended target for new UI work.
- Do not add or use Nightingale until the project owners confirm a package version compatible with React 19 and provide access to its package feed. The currently available compatibility information lists React 16–18 only.
- Once compatibility and feed access are confirmed, verify them using the package's authoritative metadata and the project's configured registry before adding the dependency. Do not silently downgrade React or substitute another component library.
- Until then, use the [Nightingale Storybook](https://storybook.bswsites.com/?path=/docs/get-started-about-nightingale--page) as a visual and documentation reference for foundations, components, patterns, and accessibility guidance.
- In this reference mode, native React, HTML, and CSS may be used for temporary previews. Label them as approximations, not official Nightingale components; do not imply their APIs or behavior match the library.
- Keep the preview renderer behind a small adapter boundary so it can be connected to the official package after compatibility and feed access are confirmed.
- Before automating Storybook ingestion, verify that an officially supported machine-readable catalog is available. Do not depend on undocumented endpoints.
- If a task specifically requires actual Nightingale components, stop and report the unresolved version or access requirement.

## Project structure

- Create directories only when a requested implementation needs them; do not rely on presumed `app` or `desktop` directories.
- Keep setup instructions and generated code aligned with the actual repository structure and available tooling.
