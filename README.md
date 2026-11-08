# Finanças Teste

Download-only distribution for the macOS test app. This repository contains public release builds, installation notes and a signed Sparkle update feed; it does not contain the app source code or anyone’s financial records.

## Install once

Download the latest universal ZIP from [Releases](https://github.com/rodrigosouzah/financas-test-updates/releases/latest), unzip it, and replace **Financas Teste.app** in Applications. Keep the same app name and do not delete your profiles or use the expense reset.

Install version **0.2.1 or newer** once to get the stable update feed, installed-version label in the bottom-right corner, and bell notifications with a **Baixar nova versão** link. Version 0.1 cannot update itself. Version 0.2 used a latest-download feed address that returned timeouts and is superseded by 0.2.1. Later releases check automatically; manual checking is in the app menu under **Buscar atualizações…**. Downloads and the update feed are signed with the app’s update key. Editing code alone does not publish an update: each new build is packaged, signed and released.

The stable feed is [appcast.xml](https://raw.githubusercontent.com/rodrigosouzah/financas-test-updates/main/appcast.xml). Public download hashes and signatures were verified after publication; end-to-end updating on the tester’s Mac still needs validation.

## Data

Entries, imported rows, registered cards, people, savings goals, widget order and visibility remain in the existing local profile directory on each Mac. Updates replace the application bundle. They do not upload or overwrite local profile data. Cloud profile synchronization is not implemented.

## Test distribution

Requires macOS 14 or newer; supports Apple silicon and Intel Macs. This beta is locally signed and is **not Apple-notarized**. If blocked, follow [Apple’s Open Anyway instructions](https://support.apple.com/102445) only if you trust the sender. Do not disable macOS security protections.
