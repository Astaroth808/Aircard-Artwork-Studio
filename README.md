# Aircard Artwork Studio

An offline, single-file web tool for preparing card artwork for **AirCard**. Choose an image, frame it, and export a **1536 × 969 PNG** ready to import into AirCard.

Everything runs locally in your browser. Images are never uploaded, and the page makes no network requests.

## Use it

1. Download `index.html`.
2. Open it in a current browser (Chrome, Edge, Firefox or Safari). No install, account or internet connection is needed.
3. Choose, drop or paste (Ctrl/⌘+V) a PNG, JPEG or WebP image.
4. Adjust the framing, then click **Download artwork PNG**.
5. In AirCard, select the exported PNG, preview it and apply it.

## Features

- **Scale-to-fill framing** that matches AirCard's own centre-crop geometry, with zoom up to 4×.
- **Framing controls:** drag to move, mouse wheel or pinch to zoom around the cursor, arrow keys to nudge, `+` / `−` to zoom and `0` to reset. Sliders are also available.
- **Transparency handling:** keep the alpha channel, or fill with white or black.
- **Resolution warning** when the crop has to be enlarged past 100% and may look soft.
- **Large-image safety:** files over 30 MiB, 48 MP or 16,384 px per side are rejected from the file header, before the image is decoded.
- **Fast on big photos:** pre-scaled copies keep dragging smooth, and the export is pixel-identical to the preview.

## Languages

繁體中文（香港）, 繁體中文（台灣）, English, 日本語, 한국어, Español, Français and Deutsch.

The page picks a language from your browser settings and falls back to English. You can also choose one from the menu or force one with `?lang=`, for example `index.html?lang=ja`.

## Themes

System (follows your OS, including high-contrast mode), Light, Dark, High contrast and Sepia. You can also force one with `?theme=`, for example `index.html?theme=dark`. Text in every theme meets the WCAG 4.5:1 contrast minimum.

## Privacy

- A strict Content Security Policy blocks all network connections.
- The only data stored is your language and theme choice, kept in your browser's local storage.
- Unexported work is discarded when you close the page.

## Limitations

- The preview shows only the image area. It does not simulate Wallet's rounded corners, text or logos.
- Colours and scaling may differ slightly between your browser and your phone.
- SVG, HEIC and GIF files aren't supported. Convert them to PNG or JPEG first.

## License

Released under the [MIT License](LICENSE).

---

AirCard Guide community utility. This tool only prepares images; installing, connecting and applying artwork is done in AirCard.
