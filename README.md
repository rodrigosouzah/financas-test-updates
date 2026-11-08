# Finanças Teste

Public download-only distribution for the macOS test app. No personal financial records or app source code are published here.

## Download and install

Use [the latest release](https://github.com/rodrigosouzah/financas-test-updates/releases/latest) and download **only the Financas-Teste-…-Universal.zip** asset, not the automatically generated Source code ZIP. Unzip it, quit the old app and replace **Financas Teste.app** in Applications. Keep your profiles and do not reset expenses.

Install **0.2.2 or newer**. Version 0.2.1 had a confirmed Sparkle framework loading-path error that prevented launch; 0.2.2 corrects it. The previous failed package reproduces the library-load error, while the corrected archive passes framework resolution on both architectures and dynamic loading on Apple silicon. The tester still validates the app window and interactions.

## Features

- **0.2.3:** rename spending types through **Tipo → Editar nomes dos tipos…** in Despesas, Importar Excel or the new-expense form. Names are saved per profile and update linked entries and widgets without changing financial values.
- Despesas shows the purchase total and a separate read-only **Parcela do mês** for the selected month.
- Red row-delete controls with confirmation; Importar Excel supports cell/row selection, filling selected cells with one copied value, deleting selected rows and exporting Excel.
- Dates automatically insert slashes while typing ddmmyyyy.
- **Cartões | Contas** separates cards and bank accounts. Account cards show reported balance/date and cumulative projected balance through the selected month. The projection excludes movements already covered by the reported-balance date.
- Expenses can be allocated to a payment account; salary and other income can be allocated to a destination account.
- Brown-and-gold wallet icon, installed version at bottom right, and update notifications with **Baixar nova versão** links.

## Updates and data

The stable signed feed is [appcast.xml](https://raw.githubusercontent.com/rodrigosouzah/financas-test-updates/main/appcast.xml). Future packaged, signed and published builds can update through Sparkle; manual checking is **Buscar atualizações…** in the app menu. Editing source alone does not publish an update.

Entries, imported rows, cards, bank accounts, people, savings goals, and widget preferences remain in each Mac’s existing local profile directory. Updates replace the application bundle; no financial records are uploaded. Cloud profile sync and AI agents are not implemented.

## Test distribution

macOS 14+; universal Apple silicon and Intel. Locally signed, **not Apple-notarized**. Gatekeeper may still require [Apple’s Open Anyway procedure](https://support.apple.com/102445) until Developer ID signing/notarization is configured. Do not disable macOS security protections.
