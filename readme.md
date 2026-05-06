# did:cid Method (Technical Overview)

Spec-Up rendering of the `did:cid` technical presentation given to the
[DIF DID Methods Working Group](https://identity.foundation/working-groups/did-methods.html)
on 2026-05-06.

- **Rendered spec:** <https://flaxscrip.github.io/didcid-presentation/>
- **DIF method proposal:** [decentralized-identity/did-methods — `PROPOSAL-did-cid.md`](https://github.com/decentralized-identity/did-methods/blob/main/method-proposals/PROPOSAL-did-cid.md)
- **Normative spec & reference implementation:** [archetech/archon](https://github.com/archetech/archon)
  — see [`docs/scheme.md`](https://github.com/archetech/archon/blob/main/docs/scheme.md)
- **Source presentation:** [`docs/presentations/did-cid-technical-presentation.md`](https://github.com/archetech/archon/blob/main/docs/presentations/did-cid-technical-presentation.md)

## What this repo is

This repo is a friendlier reading surface for the `did:cid` material that
DIF members were pointed to during the meeting. The content is a rewrite
of the slide deck into a spec-style document with a table of contents,
defined terms, and stable section anchors, so it can be linked and
referenced from the DIF proposal and review threads.

It is **not** the normative protocol specification. The normative spec is
maintained in the Archon repository.

## Editing

- Source content: [`spec/spec.md`](spec/spec.md)
- Build configuration: [`specs.json`](specs.json)
- Rendered output (committed for GitHub Pages): [`docs/`](docs/)

```bash
npm install
npm run render        # one-shot build to docs/
npm run dev           # live-reload preview at http://127.0.0.1:5173
```

> **Heads up — upstream template gotcha:** the
> [`decentralized-identity/spec-up`](https://github.com/decentralized-identity/spec-up)
> template references `src/web-awesome/dist/styles/webawesome.css`, but the
> bundled directory is `src/web-awesome/dist-cdn/`. This repo carries a
> `dist -> dist-cdn` symlink so that `npm run render` works out of the box.

## License

Apache 2.0 (inherited from the spec-up template).
