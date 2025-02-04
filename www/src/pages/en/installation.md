---
title: Installation
description: Installation instructions for Create T3 App
layout: ../../layouts/docs.astro
---

To scaffold an app using `create-t3-app`, run any of the following three commands and answer the command prompt questions:

### npm

```bash
npx create-t3-app@latest
```

### yarn

```bash
yarn create t3-app
```

### pnpm

```bash
pnpm dlx create-t3-app@latest
```

## Advanced usage

| Option/Flag       | Description                                                             |
| ----------------- | ----------------------------------------------------------------------- |
| `[dir]`           | Include a directory argument with a name for the project                |
| `--noGit`         | Explicitly tell the CLI to not initialize a new git repo in the project |
| `-y`, `--default` | Bypass the CLI and use all default options to bootstrap a new t3-app    |
| `--noInstall`     | Generate project without installing dependencies                        |

## Experimental usage

For our CI, we have some experimental flags that allows you to scaffold any app without any prompts. If this use case applies to you, you can use these flags. Please note that these flags are experimental and may change in the future.

| Flag                  | Description                        |
| --------------------- | ---------------------------------- |
| `--CI`                | Let the CLI know you're in CI mode |
| `--trpc=trpc`         | Include `trpc` in the project      |
| `--prisma=prisma`     | Include `prisma` in the project    |
| `--nextAuth=nextAuth` | Include `nextAuth` in the project  |
| `--tailwind=tailwind` | Include `tailwind` in the project  |

**Note: If you don't provide the `CI` flag, the rest of these flags has no effect.**

### Example

```bash
pnpm dlx create-t3-app@latest --CI --trpc=trpc  --tailwind=tailwind
```
