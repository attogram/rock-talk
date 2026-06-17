# #107: L13 image std

Metadata:
- State: open
- Author: attogram
- Created: 2026-06-15T21:28:08Z

## Description
## Operational Standard: Image Artifact Black Footer & Fair Use Attribution

To protect repository assets from copyright drift and comply with Fair Use (17 U.S.C. § 107), all video/image screenshots used for technical taxonomy validation must feature a burned-in black footer banner before being committed to the repo.

This ensures that the academic context and legal attribution remain hardcoded into the asset's pixel data, preventing downstream multi-agent or human misconstruction.

### 1. Visual Specification
* **Layout:** Uniform solid black rectangle appended to the bottom canvas of the image artifact.
* **Text Formatting:** White, sans-serif typography, capitalized, horizontally centered, scaled for high legibility/OCR processing.

### 2. Standard Metadata Template
Replace the bracketed items with the specific archetype data for the file:

    FIGURE [X.X]: [ARCHETYPE VECTOR TYPE AND PROPER NAME]. COPYRIGHT © [YEAR] [COPYRIGHT HOLDER / STUDIO]. ACADEMIC COMMENTARY / FAIR USE STUDY.

### 3. Canonical Example (The Malone Vector)
For the current *The Office* media captures, use this exact string in the image footer:

    FIGURE 2.1: TYPE II (MALONE VECTOR) LITE SCP MANIFESTATION. COPYRIGHT © 2011 NBCUNIVERSAL MEDIA, LLC. ACADEMIC COMMENTARY / FAIR USE.

## Comments
