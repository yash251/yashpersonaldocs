# Subgraph Handbook

A practical guide to building, deploying, and debugging subgraphs on
The Graph. Live at [yashpersonal.thally.app](https://yashpersonal.thally.app).

Built with [Thally](https://thally.io) for the Thally Developer Experience
assessment. The write-up of how this site was made, including the obstacles,
is on [dev.to](https://dev.to/0x_yasshhh_/publishing-a-docs-site-with-thally-what-worked-what-did-not-56jj).

## Pages

| Page | What it covers |
| --- | --- |
| [Introduction](src/content/introduction.mdx) | What a subgraph is and who this handbook is for. |
| [Quickstart](src/content/quickstart.mdx) | Deploy the Gravity contract subgraph to Subgraph Studio and verify it with a query. |
| [Debug a failed subgraph](src/content/guides/debug-a-failed-subgraph.mdx) | Read the indexing status, match the error to a cause, apply the fix. |

## Edit

Content lives in `src/content/`, navigation in `docs.json`, and site
identity in `src/data/site.ts`. Everything else is the pinned Thally runtime.

```bash
npm install
npx thally dev       # preview on http://localhost:3040
npx thally check     # lint content, links, and navigation
npm run build
```

Push to `main` and Thally Cloud builds and publishes the site.
