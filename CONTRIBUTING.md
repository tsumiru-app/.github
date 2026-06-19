# Contributing to Tsumiru

Thanks for your interest in Tsumiru! Tsumiru is a **client** for a [Suwayomi](https://suwayomi.org/) server — it reads from a server you run. That distinction matters for where issues belong, so please skim this first.

## Sources, extensions, and "this manga won't load"

Sources and extensions live on the **Suwayomi server**, not in Tsumiru. If a source is broken, missing, or a chapter won't download, that's almost always a server/source issue — please take it to [Suwayomi-Server](https://github.com/Suwayomi/Suwayomi-Server), not here. Tsumiru issues are about the **app**: the reader, library UI, settings, connection/auth, and platform builds.

## Reporting bugs

1. Search [existing issues](https://github.com/tsumiru-app/tsumiru/issues) first.
2. Open a bug report and include: your **Tsumiru version**, **platform** (Android/Windows/macOS/Linux/Web), your **Suwayomi server version**, clear **steps to reproduce**, and what you expected vs. what happened. Logs/screenshots help a lot.

## Requesting features

Open a feature request describing the problem you're trying to solve, not just the solution. Note whether it's something the app should do vs. something the server already handles.

## Development

Tsumiru is built with Flutter.

- Flutter **3.32.4** / Dart **3.8.1** (pinned).
- Install deps: `flutter pub get`.
- After changing `@riverpod` annotations or `*.graphql` files, regenerate: `dart run build_runner build --delete-conflicting-outputs`.
- Run against a real Suwayomi server (set the server URL in **Settings → Server**).
- Match the surrounding code style; keep PRs focused and reference the issue they address.

## Pull requests

- One logical change per PR; describe the *why*.
- Make sure it builds and you've tested the affected flow.
- By contributing, you agree your work is licensed under the project's **MPL-2.0** license.

Please also follow our [Code of Conduct](./CODE_OF_CONDUCT.md).
