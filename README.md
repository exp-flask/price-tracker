This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.tsx`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.ts`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.


##From Scratch
New Next.js project:
```npx create-next-app@latest ./```
`./` specified to not create under a new project name, instead create on current dir (avoids duplication)


##Node Version and fnm
There are a couple node version managers out there like `nvm` and `fnm`. This project uses the Rust based `fnm`, which focuses on project dir scope rather than globally like nvm.

###Setting up fnm on this local project
If not already installed, install via package manager: `choco install fnm` (Windows) or `brew install fnm` (macOS)

Set desired node version in a new .node-version file: 
```echo "v21.7.2" > .node-version```
(optional) peruse available versions `fnm list-remote` and `fnm install [version]` if your not sure

auto-switch to node version via fnm when navigating to directory:
Windows (PowerShell)
```fnm env --use-on-cd | Out-String | Invoke-Expression```
macOS (zsh)
```eval "$(fnm env --use-on-cd)"```
If version not already installed, answer `y` to prompt

Check versions were updated with `fnm current`, `node -v`, `npm -v`