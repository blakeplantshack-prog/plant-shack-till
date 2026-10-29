# Plant Shack Till

A simple till for The Plant Shack, Deception Bay. It is one web page (`index.html`) served by GitHub Pages. Each till keeps its own sales in Chrome on that computer.

## Setting up a till computer

1. **Receipt printer:** set it as the Windows default printer.
2. **Cash drawer:** plug it into the receipt printer. In the printer's Windows settings (Printing preferences), turn on "open cash drawer" when printing.
3. **Zebra sticker printer:** install Zebra Browser Print and leave it running. In the till, go to Stickers → Sticker printer settings and pick the Zebra.
4. **Scanner:** plug it in. It types into the scan box like a keyboard.
5. **Desktop shortcut for the till (receipts print with no print window):**
   `"C:\Program Files\Google\Chrome\Application\chrome.exe" --kiosk-printing --app=https://blakeplantshack-prog.github.io/plant-shack-till/`
6. The first time it opens, Chrome may ask to let the page reach devices on this computer. Say **Allow**, because that is how stickers reach the Zebra.
