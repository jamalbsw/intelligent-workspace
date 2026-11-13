# AEL Prototype Studio

A shared workspace starter for turning product requests into interactive
prototypes, using the Nightingale Storybook as a temporary design reference.

**GitHub Pages:** [Open the prototype studio](https://jamalbsw.github.io/intelligent-workspace/)

The site will be available after the GitHub Pages workflow completes its first
successful deployment. In the repository settings, set **Settings → Pages →
Build and deployment → Source** to **GitHub Actions**.

## Run locally

```sh
cd apps/web
npm ci
npm run dev
```

See [the web app README](./apps/web/README.md) for checks and current limitations.

Generated previews are temporary approximations, not official Nightingale
components. AI generation, sign-in, and shared storage are not connected yet.
Use fictional examples only; do not enter patient or confidential information.
