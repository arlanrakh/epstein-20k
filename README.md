---
tags:
- epstein
- public-records
- government-documents
- legal-documents
- research
- information-retrieval
---
# Disclaimer
This dataset is a reupload of a previously circulating public dataset. The contents may include unverified, incomplete, disputed, or inaccurate information and should not be interpreted as factual, authoritative, or as proof of guilt for any individual.
This dataset is provided strictly for research, archival, and educational purposes, such as analysis of information propagation, data preservation, or media studies.
No claims are made regarding the accuracy, authenticity, or legitimacy of the materials contained herein.
If the dataset is demonstrated to be falsified, inaccurate, or if the original creator or relevant rights holders request removal, it will be taken down promptly.
This dataset should not be relied upon as a source of truth. The maintainer of this repository does not endorse, affirm, or validate any claims contained within the dataset. This reupload is intended solely to preserve access to publicly released materials in their extracted text form. The rest of this readme is a copy of the original repository.

# U.S. House Oversight Epstein Estate Documents

The motivation for curating this dataset is to enable transparent exploration of the Epstein estate documents. 
The goal is to empower AI practitioners, researchers, and enthusiasts to build RAG based systems 
that can identify patterns, connections, and insights that are difficult to obtain through manual inspection.

## Usage and Responsibilities (Required Reading)

This dataset is provided for **research and exploratory analysis** with a focus on:

- Evaluating information retrieval and retrieval augmented generation (RAG) systems.
- Developing and testing search, clustering, and summarization methods on a real world corpus.

**Users are responsible for:**

- Using the dataset only for lawful purposes and in accordance with institutional and ethical review requirements.
- Treating individuals mentioned in the documents with respect, and avoiding sensationalism or misuse of sensitive material.
- Clearly distinguishing model generated content and exploratory findings from verified facts, and citing primary sources where appropriate.

It is **not** intended for:

- Fine-tuning language models.
- Harassment, doxing, or targeted attacks on any individual or group.
- Attempts to deanonymize redacted information or circumvent existing redactions.
- Making or amplifying unverified allegations as factual claims.
  
All use must comply with applicable law, institutional policies, and the terms of the original House releases. See the “Legal and copyright status” and “Ethical and content warning” sections below before working with this corpus.


## Source (All data derived from publicly released materials)

All documents originate from the public release **“Oversight Committee Releases Additional Epstein Estate Documents”** on the official House Oversight Committee website (press release dated **November 12, 2025**):

https://oversight.house.gov/release/oversight-committee-releases-additional-epstein-estate-documents/

The underlying materials are distributed via a Google Drive structure maintained by the Committee. This dataset is an independent derivative collection built from that release and is **not** an official product of the U.S. House of Representatives or the Committee on Oversight and Government Reform.


## Dataset contents

- **Documents**: Over 25,000 plain text files derived from the committee’s public releases organized in a single csv file
- **Source Folders**:
  - `TEXT/` – Files that were originally text-based (e.g., PDFs, emails) and converted to plain text.
  - `IMAGES/` – Image files (primarily JPG) converted to text via OCR.

**Filenames preserve the relative path and naming conventions from the original Google Drive release, to facilitate cross-referencing back to the official source files.**


## Processing

- All image files under the `IMAGES/` directory (approximately 20,000 JPGs) were converted to machine-readable text using the open-source **Tesseract** OCR engine.
- Native text-based files under `TEXT/` were converted to plain text using standard tools (e.g., PDF/text extraction) without manual editing.
- No manual content editing, summarization, or redaction has been performed beyond:
  - basic file organization,
  - text extraction / OCR,
  - and any redactions already present in the official House releases.

As a result, the corpus may contain:

- OCR noise and misrecognized characters
- Broken formatting
- Redaction blocks, stamps, or markers inherited from the original scans

## Legal and copyright status (non-authoritative)

- The original underlying documents were created by various private individuals and entities, not by the dataset maintainer.
- The documents are sourced from releases published by the U.S. House Committee on Oversight and Government Reform. The release webpages themselves carry standard copyright notices (© 2025 Committee on Oversight and Government Reform), and many individual documents are likely protected by copyright held by their original authors or rights holders.
- This dataset:
  - **Does not** assert any ownership over the underlying documents.
  - **Does not** grant any license to reproduce, distribute, or create derivative works from the underlying texts beyond what may already be permitted by law (e.g., fair use or similar doctrines in your jurisdiction).
- Users are solely responsible for ensuring that their use of this corpus complies with applicable copyright law, privacy law, institutional policies, and the terms of the original House releases.

Nothing in this dataset card constitutes legal advice. If you plan to use this corpus in a public-facing product, for model training, or at scale, you should seek independent legal counsel.

## Ethical and content warning

The documents contain material related to:

- Sexual abuse and exploitation
- Trafficking
- Violence and other highly sensitive topics
- Unverified allegations, opinions, or speculation


## Intended use and limitations

Recommended / common use cases include:

- Text mining and exploratory analysis of the *public record* surrounding the Epstein estate documents.
- Search / retrieval experiments (e.g., indexing, ranking, IR/RAG prototypes) conducted in controlled or research settings.
- Qualitative review by journalists, historians, or legal scholars.# epstein-20k
