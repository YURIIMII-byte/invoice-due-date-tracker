# invoice-due-date-tracker

OCRs a photographed invoice and logs vendor, amount, and due date so nothing is paid late, on-device. Built with [Tether's QVAC SDK](https://github.com/tetherto/qvac) — the model runs on-device, so nothing leaves your machine.

## What it does

OCRs a photographed invoice and logs vendor, amount, and due date so nothing is paid late, on-device.

**QVAC functions used:** `loadModel`, `ocr` and `completion`.

![invoice-due-date-tracker demo](demo.png)

## Why I built it

Late fees are a tax on paper invoices sitting in a pile.

## Requirements

- Node.js >= 22
- `@qvac/sdk` `^0.19.0` (installed automatically via `npm install`)

## Install

```bash
git clone https://github.com/YURIIMII-byte/invoice-due-date-tracker.git
cd invoice-due-date-tracker
npm install
```

## Run

```bash
node index.js path/to/invoice.jpg
```

See the comments at the top of `index.js` for the exact input this app expects. On first run, QVAC downloads the model it needs once and caches it locally; every run after that is fully offline.

## SDK version used

`@qvac/sdk` `0.19.1`

## License

MIT — see [LICENSE](LICENSE).
