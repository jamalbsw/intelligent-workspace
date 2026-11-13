# AEL Prototype Studio

The first web workspace for collecting prototype requests and previewing the
generation flow. It uses the public Nightingale Storybook as a design reference;
it does not import or claim to render official Nightingale components.

## Run locally

```sh
npm install
npm run dev
```

Run checks with:

```sh
npm run build
npm run lint
```

## Current limitations

- The AI generation service is not connected, so the Generate button is
  intentionally disabled.
- Authentication, shared team storage, and prototype versioning are not
  connected yet.
- Use fictional examples only. Do not enter patient or confidential information.
- Temporary previews must be identified as approximations until the official
  Nightingale package is approved and available.
