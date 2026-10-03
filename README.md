# Real Time Crypto Fraud Attribution System

An interactive cryptocurrency investigation demo based on the ChainTrace architecture roadmap. All wallets, transfers, service labels, findings and watch events are synthetic.

## Open the demo

1. Extract the ZIP folder.
2. Open `index.html` in Chrome, Edge, Firefox or another modern browser.

No installation or API key is required. Dark mode is enabled by default; the top-right button switches between dark and light and remembers your preference when browser storage is available. Google Fonts loads when an internet connection is available; otherwise the site uses local fallback fonts.

## Optional local server

If Node.js is installed, open a terminal in this folder and run:

```sh
node server.cjs
```

Open http://127.0.0.1:4173 in your browser. Press Ctrl+C in the terminal to stop the server. The server accepts connections only from your own computer. If that port is already in use, choose another one:

```sh
node server.cjs 4174
```

## Project files

- `index.html`: page structure and demo views.
- `style.css`: responsive styling and dark/light themes.
- `app.js`: synthetic data, graph controls, evidence, notes, alerts and report export.
- `server.cjs`: optional local development server; no external dependencies.

## Try the workflow

1. Click **How it works** for an introduction.
2. Open **Workspace**, select wallets in the graph, and use **View supporting evidence**.
3. Compare **All paths** with **Service path**, or change the displayed hop depth.
4. Select **Add analyst note** to record your assessment.
5. Open **Watch alerts** and select **Replay new activity**.
6. Select **Export report** to download an HTML report. Open that report and choose **Print / Save as PDF**.
7. **New demo case** lets you rename the case while reusing the same synthetic scenario.

## Demo boundaries

- This is a browser-based prototype, with no backend or database.
- Case changes, analyst notes and alerts last only for the current page session. Export before refreshing or closing the page.
- Reports remain unapproved drafts; there is no approval/sign-off workflow.
- No live blockchain provider, live AI analysis, background watcher, cross-chain tracing, NCRP or SAHYOG connection is included.
- The priority score is a fixed demonstration value, not a probability of fraud.
- A transaction path does not prove the same funds moved through all transfers. A service label does not identify a customer.
- Optional browser WebMCP tools are registered only when the browser supports them. Ordinary manual use does not require WebMCP.

## Editing and hosting

Edit the three website files in any text editor and refresh the browser. The website is plain HTML, CSS and JavaScript, with no build step. You can deploy these three files to a static hosting provider. This download contains no hosting credentials or account-specific deployment configuration.
