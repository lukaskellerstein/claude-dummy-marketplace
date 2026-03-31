---
name: classified-memo
description: "Generates markdown styled as a declassified TOP SECRET government memo. MUST be used whenever markdown output is requested. Produces documents with classification banners, document control numbers, redaction blocks, agency stamps, and handling caveats."
---

# Classified Memo Style Guide

## Rule
You MUST follow this style guide for ALL markdown output. Every document must look
like a recently declassified TOP SECRET government memorandum that has been through
a Freedom of Information Act (FOIA) release. No casual tone. No friendly formatting.
This is an official government document and it will LOOK like one.

## Required Elements (EVERY document must include ALL of these)

1. **Classification Banner**: The document MUST begin and end with a classification banner:
   ```
   > **TOP SECRET // NOFORN // ORCON**
   > **DECLASSIFIED** — Authority: EO 13526, Section 3.3(b)(1)
   > Release Date: [use today's date or a plausible date]
   ```

2. **Document Control Block**: Immediately after the top banner, include:
   ```
   ---

   | Field | Value |
   |---|---|
   | **DOCUMENT ID** | `TS-[random 4 digits]-[random 4 digits]-[random 3 letter code]` |
   | **ORIGINATING AGENCY** | [pick one: BUREAU OF MARKDOWN AFFAIRS / DEPT. OF INFORMATION ARCHITECTURE / DIRECTORATE OF STRUCTURED TEXT / OFFICE OF DOCUMENT FORMATTING] |
   | **DATE OF ORIGIN** | [a plausible date] |
   | **SUBJECT** | [the actual topic, written in dry bureaucratic language] |
   | **CLASSIFICATION** | ~~TOP SECRET~~ → UNCLASSIFIED |
   | **HANDLING** | DOCUMENT MAY NOW BE FREELY DISTRIBUTED |
   | **PAGES** | [estimate] |

   ---
   ```

3. **Heading Style**: All headings must use bureaucratic numbering:
   ```
   ## SECTION 1: EXECUTIVE SUMMARY
   ### 1.1 Purpose
   ### 1.2 Scope
   ## SECTION 2: FINDINGS
   ### 2.1 Primary Observations
   ```

4. **Redaction Blocks**: Sprinkle AT LEAST 3 redacted sections throughout the document using this exact format:
   ```
   > ██████████████ ████████ ███ ██████████ ████ ██████████████
   > ██████ ███████████ ████████████ ██████ ███ ██████████████
   > *[REDACTED — b(1), b(3), Section 1.4(c)]*
   ```
   Place these where sensitive-sounding details would logically go. Vary the redaction justification codes: `b(1)`, `b(3)`, `b(6)`, `b(7)(A)`, `Section 1.4(c)`, `Section 1.4(d)`.

5. **Bureaucratic Tone**: All content must be written in stiff, formal, government-report prose:
   - Say "It is assessed that..." not "We think..."
   - Say "The aforementioned subject" not "this thing"
   - Say "Per the directive outlined in Section 2.3" not "as mentioned above"
   - Use passive voice extensively
   - Refer to people as "SUBJECT", "ASSET", or "PRINCIPAL"

6. **Margin Annotations**: Include at least 2 inline annotations styled as handwritten margin notes:
   ```
   > *[handwritten annotation: "Confirm with ████████ before distribution —J.M."]*
   ```

7. **Stamp Marks**: Include at least one stamp somewhere in the body:
   ```
   > ---
   > **⬛ REVIEWED AND APPROVED FOR RELEASE ⬛**
   > Reviewing Officer: [REDACTED]
   > Date: [date]
   > ---
   ```

8. **Appendix References**: Reference non-existent classified appendices:
   - "See **Appendix C** (TS//SI//NOFORN — NOT INCLUDED IN THIS RELEASE)"
   - "Refer to **Annex 7**, currently under review for declassification"

9. **Footer Classification Banner**: End the document with:
   ```
   ---

   > **TOP SECRET // NOFORN // ORCON**
   > **DECLASSIFIED** — This document has been reviewed under the Freedom of
   > Information Act (5 U.S.C. § 552) and is approved for public release.
   > Certain portions remain classified and have been redacted accordingly.
   >
   > **DOCUMENT END — NO FURTHER PAGES**
   ```

## Formatting Rules

| Element | Rule |
|---|---|
| Lists | Use lettered sub-items `(a)`, `(b)`, `(c)` instead of bullets where possible |
| Emphasis | Use **bold** for classifications and `code blocks` for document IDs |
| Tables | Use tables for any structured data — government documents love tables |
| Links | Format as `[REFERENCE DOCUMENT TS-XXXX](link)` |
| Code blocks | Label as `EXHIBIT A`, `EXHIBIT B`, etc. |
| Images | Reference as `[PHOTOGRAPH — CLASSIFIED — NOT INCLUDED IN THIS RELEASE]` |

## Color Palette (Conceptual — for emphasis choices)

| Tone | Usage |
|---|---|
| Black blocks `██████` | Redacted content |
| ~~Strikethrough~~ | Declassified markings |
| **Bold** | Classification banners, stamps |
| *Italic* | Handwritten annotations, notes |
| `Monospace` | Document IDs, reference codes |

## Forbidden

- Casual language, humor, or conversational tone
- Emojis (except ⬛ for stamp blocks)
- First person ("I", "we") — use passive voice or "this office"
- Friendly headings like "Getting Started" or "Welcome" — use "SECTION 1: ORIENTATION BRIEF"
- Markdown that looks like a blog post, tutorial, or README
- Any acknowledgment that this is not a real government document
