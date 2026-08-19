# MyZubster Web

> 🌍 **Understand MyZubster in your language:** [Global multilingual guide](https://github.com/MyZubster-Ecosystem/myzubster/blob/main/docs/i18n/README.md) — English, Italiano, Español, Français, Deutsch, Português, 中文, 日本語, 한국어, العربية, हिन्दी, Русский, Türkçe, Bahasa Indonesia, Polski, Українська, বাংলা, اردو, فارسی, Kiswahili.
>
> MyZubster connects real-world observations, verifiable evidence, collaborative bounties and platform rewards. **MYZ is currently an internal reward/accounting ledger; external XMR/token/blockchain settlement is separate and independently verified.**

Public web-presence repository for the MyZubster ecosystem.

## Community

- 🌐 [MyZubster Community Hub](https://coal-lilac-ef7.notion.site/MyZubster-Community-Hub-3c1b5d1556838132af4cc7cb258d60ec)
- 💬 [Join the MyZubster Slack community](https://join.slack.com/t/nuovaareadila-ml19359/shared_invite/zt-47dxpvwio-ZIkNdYv5Uk_glAilUiVnkg)

Use the Community Hub for contributor onboarding, public documentation and ecosystem guidance. Use Slack for discussion and contributor coordination.

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
