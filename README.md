# Plant Shack Till

A simple till for The Plant Shack, Deception Bay. It is one web page (`index.html`) served by GitHub Pages. Each till keeps its own sales in Chrome on that computer.

## Setting up a till computer

1. **Receipt printer:** set it as the Windows default printer.
2. **Cash drawer (Epson TM-T82IV):** plug the drawer cable into the DK port on the back of the printer. Install the Epson Advanced Printer Driver (APD), then in Windows open Printers → the Epson → Printing preferences, find the Cash Drawer setting and set drawer #1 to open **before printing**. The drawer then opens whenever something prints: cash sales print a receipt automatically, and OD with no sale prints a small "No sale" slip.
3. **Zebra sticker printer:** install Zebra Browser Print and leave it running. In the till, go to Stickers → Sticker printer settings and pick the Zebra.
4. **Scanner:** plug it in. It types into the scan box like a keyboard.
5. **Desktop shortcut for the till (receipts print with no print window):**
   `"C:\Program Files\Google\Chrome\Application\chrome.exe" --user-data-dir="C:\PlantShackTill" --kiosk-printing --app=https://blakeplantshack-prog.github.io/plant-shack-till/`
   The separate profile (`--user-data-dir`) makes the no-print-window setting work even when Chrome is already running. If the shortcut won't open, use `Program Files (x86)` instead.
6. The first time it opens, Chrome may ask to let the page reach devices on this computer. Say **Allow**, because that is how stickers reach the Zebra.
