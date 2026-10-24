<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Offline Translation, Read-Aloud and Accessibility

OYYO NotzUP translates supported text results on the Android device. The captured source is not uploaded to a cloud AI service for translation, style processing, read-aloud or correction memory.

## Translate a result

1. Open a file with a transcript, visible text, visual note, summary or another supported text result.
2. Choose **Translate offline**.
3. Select the destination language. The required ML Kit language pack downloads on first use and is then used locally.
4. Select a translation profile.
5. Review names, numbers, technical terms, quoted material and culturally sensitive phrases against the source.
6. Copy the result, or choose **Edit & approve** to correct it.

Long text is translated in bounded paragraph-sized passages. Headings, lists and nearby sentences remain together where possible instead of being sent one isolated line at a time.

## Translation profiles

- **Faithful:** direct local translation with the original structure preserved.
- **Natural context:** keeps paragraphs, lists and punctuation together, then normalizes the result for easier reading.
- **Playful:** a light wording profile available for English and Italian.
- **Napoletano · beta:** experimental local styling applied after Italian translation.
- **Barese · beta:** experimental local styling applied after Italian translation.

The beta regional profiles intentionally use a conservative, limited vocabulary. They do not claim to replace a native speaker or the broader intent, culture and dialect capability described by [OYYO Language](https://oyyo.one/language). Review them before sharing.

## Private correction memory

Choose **Edit & approve** when a result needs correction. NotzUP stores only the corrected output for that exact source, destination language and selected profile in private application storage on the device. The same combination can then reuse the approved correction without sending it to a server.

An approval is not a global dictionary change. A different source, target language or profile is translated and reviewed separately.

## Listen to a result aloud

1. Open a populated result section.
2. Choose **Listen aloud**.
3. NotzUP selects an installed offline Android voice that matches the detected language where available.
4. Choose **Stop reading** to end playback immediately.

If Android has no offline voice for that language, install one through the device text-to-speech settings. NotzUP does not silently switch this feature to a network-only voice.

## Screen readers, scaling and adaptive layouts

- Primary controls and capture states expose spoken labels for Android screen readers.
- The interface follows Android display-size and font-size settings.
- Touch controls adapt to phones, tablets and foldables.
- Barcode manual and automatic controls remain beside the camera rather than being hidden under the results panel.
- Google TV is intentionally excluded because the mobile workflow requires touch and camera interaction.

## Privacy checklist

- Translation input and output stay on the device.
- Translation packs are downloaded model files; captured content is not sent with the model download.
- Approved correction memory stays in the app's private local storage.
- Read-aloud uses an installed offline voice.
- Data leaves the device only after a separate user-selected online action, such as sharing, online barcode search, an authorized connector or encrypted backup.

## Troubleshooting

### The language pack will not install

Check the internet connection and free device storage, then retry the target language. The initial model download needs network access; later supported translations can run locally.

### A dialect phrase looks wrong

Treat the beta profile as a draft. Correct it, approve the exact result if useful, or switch to **Faithful** or **Natural context**. Use a native reviewer when meaning, tone or public publication matters.

### Read-aloud offers no suitable voice

Install an offline voice for the result language in Android text-to-speech settings. Restart the app after the voice package is ready.

### Text is clipped at a large font size

Rotate the device or use a larger tablet/foldable layout, then report the exact screen and Android display/font settings without attaching private captured content.

## Related guides

- [Complete User Guide](USER_GUIDE.md)
- [Local-First Privacy and Data Control](LOCAL_FIRST_PRIVACY.md)
- [Mobile Barcode and QR Inventory](MOBILE_BARCODE_INVENTORY.md)
- [Encrypted Backup and Cloud Storage](ENCRYPTED_BACKUP_AND_STORAGE.md)
- [FAQ](FAQ.md)
