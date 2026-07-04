# Privacy Policy for CatsRead

**Last updated:** July 4, 2026

CatsRead does not collect, store, or transmit any personal data. The app is fully offline and operates entirely on your device.

## Data Storage

CatsRead stores the following data locally on your device only:

- **EPUB files** you import are saved in the app's Documents directory.
- **Book covers and extracted text** are cached locally for performance.
- **Reading progress** (your current page) is saved locally.
- **Tracked vocabulary words** (words you tap while reading) are stored in a local SQLite database, including the word, language, knowledge level, and view count.
- **Reader settings** (font, size, spacing, theme) are stored in UserDefaults.
- **Per-book translation language preferences** are stored in UserDefaults.

None of this data is ever sent to us or any third party. You can delete all of it by deleting the app.

## Third-Party Libraries

CatsRead uses the following open-source libraries, all of which process data exclusively on-device:

- **GRDB** — SQLite database access
- **ZIPFoundation** — EPUB file extraction
- **Fuzi** — XML/HTML parsing

None of these libraries transmit any data.

## Apple Frameworks

CatsRead uses the following Apple frameworks:

- **Translation** — When you tap a word and request translation, the word and its surrounding sentence may be processed by Apple's on-device or server-side translation service. You can manage installed translation language packs in iOS Settings > General > Apple Intelligence & Siri > Translation.
- **NaturalLanguage** — Language detection and lemmatization. Runs entirely on-device.
- **AVSpeechSynthesizer** — Text-to-speech for word pronunciation. Runs entirely on-device.
- **UIReferenceLibraryViewController** — System dictionary lookup. Runs entirely on-device.

## No Data Collection

CatsRead does not:
- Collect analytics or usage statistics
- Use crash reporting tools
- Display advertisements
- Make network requests
- Communicate with any server
- Access your contacts, photos, location, or any other personal data
- Share any data with third parties

## Changes to This Policy

If this policy changes, we will update the "Last updated" date. Since the app does not connect to the internet, changes will be distributed through App Store updates.

## Contact

If you have questions about this privacy policy, please contact us at:

catsread@example.com