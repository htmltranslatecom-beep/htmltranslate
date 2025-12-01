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
