<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Mobile Barcode and QR Inventory

OYYO NotzUP includes a complete mobile inventory workspace, not only a barcode-reading button. It is exclusive to the mobile app, currently available on Android, and requires a **Pro or Organization** plan. Plus and Free accounts can see the feature information but cannot start inventory scanning.

## Before you start

1. Install the current Android build from an official OYYO NotzUP release channel.
2. Sign in and allow NotzUP to refresh the account entitlement.
3. Confirm that the account has Pro, or that the selected workspace has an active Organization entitlement.
4. Allow camera access when Android asks for it.
5. Keep the camera lens clean and provide even light across the code.

## Scan one barcode or QR code

1. Open **Capture** and choose **Barcode and QR**.
2. Select **Single**.
3. Choose a scan profile: all supported codes, retail products, QR codes or warehouse codes.
4. Place the code inside the frame.
5. Tap **Scan code**. NotzUP does not scan merely because a code enters the camera view.
6. Review the decoded value and format.
7. Use **Copy** to copy the exact value, or **Search online** to open a web search for that code.

An online search is an explicit browser action. The scanned value is sent to the selected search provider only after the user chooses Search online.

## Count an inventory manually

1. Select **Inventory**.
2. Tap the inventory title to give the session a useful name, such as `Warehouse A, aisle 4`.
3. Choose the most specific scan profile for the labels being counted.
4. Place one code inside the frame and tap **Scan code**.
5. Repeat for every physical item.
6. Watch the total scan count, unique-code count and quantity for the latest code.
7. If the same code is scanned again, NotzUP increases its quantity and keeps the chronological scan event.

Manual mode is the safest choice when several labels may be visible at once. No tap means no scan.

## Use controlled automatic scanning

1. Open **Inventory** and select the correct profile.
2. Tap **Start auto scan** only when the camera is aimed at the intended counting area.
3. Move each code through the frame one at a time.
4. Use the on-screen status and count feedback to confirm every accepted scan.
5. Tap **Stop auto scan** before moving through an area containing labels that should not be counted.

Automatic scanning is deliberately locked behind Start and Stop. It does not run continuously in the background.

## Import a CSV or Excel catalog

NotzUP accepts CSV and supported Excel files. The first row must contain column names. A practical template is:

| Description | Article ID | Barcode | Quantity | Warehouse | Unit |
| --- | --- | --- | ---: | --- | --- |
| Blue storage box | BOX-BLU-01 | 0012345678905 | 24 | Dubai A1 | pcs |
| USB-C cable 1 m | CAB-USBC-1M | 6299200000208 | 60 | Dubai B3 | pcs |

Recognized barcode headings include **Barcode**, **Bar code**, **EAN**, **UPC**, **Product code**, **QR** and **QR code**. Keep barcode cells as text when leading zeroes matter.

To compare a catalog:

1. Open the inventory session.
2. Tap **Import CSV or Excel catalog**.
3. Select the file from Android's document picker.
4. Review the imported item count.
5. Scan the physical stock.
6. Compare each line's expected quantity, scanned quantity and difference.

NotzUP classifies lines as matched, short or over. Scanned codes absent from the catalog appear as unlisted items instead of being discarded.

## Understand the comparison

- **Expected quantity:** the quantity imported from the catalog.
- **Scanned quantity:** the number counted during this session.
- **Difference:** scanned minus expected.
- **Updated quantity:** a warehouse-friendly output column containing the new counted value.
- **Unknown or unlisted item:** a scanned code that did not exist in the imported catalog.

Always review differences before importing the result into another stock system. NotzUP does not silently change an external warehouse database.

## Export the result

### CSV

Use CSV when another inventory or warehouse system accepts a simple update file. The export contains description, article ID, barcode, expected quantity, scanned quantity, difference, status, location, unit and updated quantity.

### Excel

The Excel export contains a catalog comparison plus detailed scan and totals information. Repeated scans are preserved in the scan sheet while totals remain grouped by code.

### PDF

The branded PDF is designed for review and printing. It includes inventory totals, matched/short/over counts, item-level differences and unlisted codes.

## Back up or restore an inventory

1. Configure encrypted backup from the account security area and import the recovery key on the phone.
2. From the inventory workspace, choose **Back up to cloud**.
3. Select the personal or Organization storage space.
4. On another authorized installation, import the same recovery key and open **Restore**.
5. Choose the dated inventory backup.
6. Confirm replacement of the current local inventory only after checking its name, scan count and catalog size.

The backup is encrypted on the device before upload. Read [Encrypted Backup and Cloud Storage](ENCRYPTED_BACKUP_AND_STORAGE.md) before depending on recovery.

## Troubleshooting

### The scanner is locked

Refresh the account entitlement and confirm the exact plan is Pro or Organization. Plus does not include barcode inventory.

### A code is visible but not read

- Select the correct format profile.
- Fill more of the frame with the code without cutting off its edges.
- Avoid glare and motion blur.
- Turn on the torch when useful.
- Try manual Scan code after the camera has focused.

### The count increased twice

Stop automatic scanning when repositioning an item. In manual mode, tap once per physical unit. Review the recent scan list before export.

### Leading zeroes disappeared during catalog import

Format barcode cells as text in the source spreadsheet, save again, and re-import it.

### The exported quantity is not in my warehouse system

NotzUP creates a reviewed export; it does not write directly into third-party inventory databases. Import the CSV or Excel file using that system's documented mapping and approval process.
