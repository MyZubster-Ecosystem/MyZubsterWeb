# MyZubster Web

Public web-presence repository for the MyZubster ecosystem.

## Status

**Bootstrap / synchronization required.** The repository was empty when the ecosystem structure was audited. The live/deployed website must not be assumed to match this repository until its source, build configuration and deployment process are intentionally synchronized.

## Intended responsibility

This repository should eventually contain the web-facing MyZubster experience or a clearly documented deployment wrapper, including:

- source code and assets;
- development/build instructions;
- environment-variable contract;
- deployment procedure;
- links to the core API and public IPFS state where appropriate;
- no production secrets.

## Architecture

The web client is a user-facing layer and must not become the authority for bounty approval or settlement state.

```text
Browser
  -> MyZubster Web
  -> Core/Gateway APIs
  -> public IPFS/IPNS data when applicable
```

## Bounties

Web work may be tracked as GitHub bounty issues for UI, accessibility, documentation and API integration.

- [Canonical Bounty System](https://github.com/MyZubster-Ecosystem/myzubster/blob/main/BOUNTIES.md)
- [Ecosystem Architecture](https://github.com/MyZubster-Ecosystem/myzubster/blob/main/docs/ECOSYSTEM.md)

Issue closure/PR merge does not prove external payment. MYZ in the current core platform is an internal reward/accounting ledger.

See `BOUNTIES.md` for local scope.

## Bootstrap checklist

- [ ] import/synchronize the actual intended web source;
- [ ] document local development;
- [ ] add `.env.example` containing placeholders only;
- [ ] document build/deploy;
- [ ] add tests/smoke checks;
- [ ] verify no server secrets are bundled into client assets.

## Related repositories

- [myzubster](https://github.com/MyZubster-Ecosystem/myzubster)
- [MyZubster-App](https://github.com/MyZubster-Ecosystem/MyZubster-App)
- [myzubster-docs](https://github.com/MyZubster-Ecosystem/myzubster-docs)
