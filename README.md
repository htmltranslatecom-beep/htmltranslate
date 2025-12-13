# 🌐 HTMLTranslate.com

**HTMLTranslate** is a completely free online HTML translator that preserves structure, tags, and inline styles.

👉 [https://htmltranslate.com](https://htmltranslate.com)

## ✨ Features
- Translate full HTML files into any language  
- Keeps structure, links, CSS classes, and inline styles intact  
- No registration, no hidden limits, no API key required  
- Works directly in your browser — nothing is stored on the server  

---
## ⚠️ Known Issues

### Position Absolute Limitation
Files containing main DOM elements with `position: absolute` style may currently fail to translate correctly. We are actively working on resolving this issue. 

**Workaround:** Consider removing or modifying absolute positioning from the main content container before translation.

---

## 📜 Changelog

### [v1.0.5] - December 2025 (13.12.2025)

#### ✨ New Features
- **Deferred Translation Links**: For longer translations (multiple languages or large files), you now receive a download link immediately. No need to wait on the page - bookmark the link and return later to download your translated files.

#### 🐛 Bug Fixes
- Fixed translation failures caused by `<noscript>` tags and other special HTML elements at the end of documents
- Resolved issue where ZIP archives were downloading with incorrect `.zip.html` extension
- Improved handling of malformed HTML files with structural errors

#### 🎨 Improvements
- Enhanced progress tracking with detailed language-by-language updates
- Added file name and target languages display on download page
- Better error handling for edge cases in HTML structure

---

### [v1.0.4] - December 2025 (07.12.2025)
#### 🛠️ Fixes
* **HTM File Translation Bug**: Fixed a critical issue where users uploading .htm files received the original untranslated file with a .html extension instead of the translated version. The system now correctly preserves the original file extension (.htm or .html) in the translated output and always returns the translated file.

### [v1.0.3] - December 2025 (03.12.2025)

#### ✨ Improvements
- 🌍 **Expanded Language Support**: Added **116 new languages** (from 134 to 250 total languages)
  - Rare African, Asian, and Oceanic languages (Acehnese, Fijian, Lingala, Tok Pisin, etc.)
  - Regional variants: French (Canada), Portuguese (Portugal), Dari
  - Dialects and scripts: Cantonese, Jamaican Patois, Malay (Jawi), Bambara (N'Ko)
  - Languages of Russia and neighboring regions: Avar, Buryat, Chechen, Tuvan, etc.


### [v1.0.2] - December 2025 (01.12.2025)

#### 🛠️ Fixes
* **File Encoding Support:** Fixed a critical issue where files with non-UTF-8 encoding (Windows-1251, ISO-8859-1, UTF-16, etc.) caused translation failures with `UnicodeDecodeError`. The system now automatically detects and handles multiple character encodings, ensuring successful processing of HTML files created in different editors and operating systems.
* **HTM File Extension Support:** Improved file type detection to properly accept both `.html` and `.htm` file extensions for translation.

#### ⚡ Improvements
* Added informational notice about static HTML file support and limitations with JavaScript-generated dynamic content
* Enhanced file reading robustness with fallback encoding mechanisms

### [v1.0.1] - November 2025 (30.11.2025)

#### 🛠️ Fixes
* **Meta Tag Removal:** Fixed an issue where translation failed due to the presence of the HTML **`content-security-policy`** meta tag in the source code. This tag is now automatically removed before processing.
* **Style and Script Preservation:** Resolved a bug causing original styles and scripts to disappear during the translation process. All essential structure, style links, and scripts are now correctly maintained in the output file.

---

## ⚙️ Use Cases
- Website localization and static page translation  
- Translating HTML email templates  
- Translating landing pages, documentation, and help files
