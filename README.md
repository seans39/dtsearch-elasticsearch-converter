# dtSearch to Elasticsearch Syntax Converter v2026 - browser-based query converter 2026

> **Turn dtSearch search expressions into Elasticsearch query string syntax entirely in your browser. Client-side conversion, readable notes, and the 2026 release.**

[![Platform](https://img.shields.io/badge/Platform-web%20browser-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/seans39/dtsearch-elasticsearch-converter?style=flat-square)](https://github.com/seans39/dtsearch-elasticsearch-converter)

---

<p align="center">
  <a href="https://seans39.github.io/dtsearch-elasticsearch-converter/">
    <img src="https://img.shields.io/badge/Download-dtSearch%20to%20Elasticsearch%20Syntax%20Converter%20Latest-brightgreen?style=for-the-badge" alt="Download dtSearch to Elasticsearch Syntax Converter">
  </a>
</p>

> **[Download Latest Build - dtSearch to Elasticsearch Syntax Converter v2026](https://seans39.github.io/dtsearch-elasticsearch-converter/)**

---

[Download Latest Build](https://seans39.github.io/dtsearch-elasticsearch-converter/)

---

## What this project is

dtSearch to Elasticsearch Syntax Converter is a web utility that maps dtSearch query syntax onto Elasticsearch query string syntax. It targets eDiscovery and litigation support work where the same search intent must travel between platforms without standing up a conversion service on a server.

All processing stays in the browser session. That keeps the path local, so you can inspect how each piece of syntax is rewritten, spot awkward edge cases, and refine queries with a clear view of what changed.

---

## Capabilities

- Maps dtSearch query syntax to Elasticsearch query string syntax
- Executes fully in the browser with no conversion backend
- Covers proximity operators, quoting, wildcards, fuzzy matching, boolean operators, and field syntax
- Calls out unsupported or ambiguous constructs for human review
- Describes rewrites and warnings in plain language
- Ships with an embedded regression self-test suite
- Fits eDiscovery and litigation support search migration
- Emphasizes private, on-device conversion only

---

## Getting started

Run it straight from a browser, or pull the repo and open the HTML entry file on your machine.

Clone:

```bash
git clone https://github.com/seans39/dtsearch-elasticsearch-converter.git
cd REPO
```

Open the main HTML file locally, or point any static file server at the folder if you want a simple local host preview.

---

## How to use it

1. Load the converter in a current web browser.
2. Enter a dtSearch query in the input field.
3. Read the Elasticsearch result plus any warnings or syntax notes.
4. Use the explanation panel to see what was transformed and why.
5. When something is marked unsupported or ambiguous, fix that fragment by hand before you reuse the query.

Typical path:

- Input: a dtSearch expression you supply
- Output: Elasticsearch query string syntax from the converter
- Side panel: warnings and plain-language explanations next to the result
- Checks: regression self-tests when you want to validate behavior

---

## Configuration

No backend is required, and setup stays minimal.

If the UI or local files expose options, keep those changes in the browser-side config the app already uses. For local work, update static paths or UI defaults in the files that ship with the repository.

---

## Requirements

- A modern web browser
- Ability to load the HTML client interface
- Disk space for the files if you download the project
- No server required for the conversion step itself
- Useful wherever you move queries between dtSearch and Elasticsearch

---

## FAQ

### Do I need network access while converting?
No. Conversion runs client-side inside the browser.

### What if a construct has no clean one-to-one mapping?
Unsupported or unclear fragments are flagged so you can handle them manually.

### How do I check behavior after a change or update?
Use the built-in regression self-test suite to compare results against expected conversions.

### Where do settings live?
On the client: in the browser session or in the local project files, depending on how you run the app.

### How should I troubleshoot a difficult query?
Start with the transformation notes, then line up the original dtSearch text with the Elasticsearch output and adjust by hand where needed.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
