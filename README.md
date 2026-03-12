# GerParlDia-MM

**GerParlDia-MM** is a multimodal diachronic corpus of German parliamentary speeches from **1949 to 2025**, designed for longitudinal research on **voice, language, and rhetorical change across decades**.

This repository serves as the project landing page and documentation hub. The accompanying website provides an overview of the dataset, including corpus scope, speaker selection principles, multimodal coverage, legal and ethical considerations, and searchable speaker-level metadata.

## Project website

The repository can be published as a static project website via GitHub Pages or GitLab Pages using the included `index.html`.

## Dataset in brief

- **Temporal coverage:** 1949-2025
- **Long-serving speakers:** 75
- **Speeches with media linkage:** 2,136
- **Modalities:** Audio, video, and text
- **Linked to OpenDiscourse:** 1,951 speeches (91.2%)

The corpus is based on official Bundestag Open Data XML metadata and persistent PoliticianID references. Where possible, records are linked to OpenDiscourse speech IDs and official plenary records. Speaker selection targets long parliamentary careers using asymmetric thresholds to account for historical gender representation.

Text and media are aligned at sentence level using a WhisperX-based pipeline. Speech boundaries are further refined using regex-based processing and LLM-assisted segmentation to remove non-speech context such as announcements.

## Main research use cases

- Voice aging and longitudinal speaker analysis
- Intra-speaker variation across decades
- Diachronic political language research
- Automatic speech recognition benchmarking
- Speaker recognition over long timespans

## Data availability

The dataset release can provide structured JSON metadata including:

- speaker-level information
- speech-level records
- complete transcripts
- persistent links or identifiers to OpenDiscourse entries
- Bundestag Mediathek media references
- archival signatures
- PDF plenary protocols

Audiovisual media files are **not redistributed** in the core release. Access to original recordings follows the official Bundestag Mediathek and Parliamentary Archive usage terms.

## Legal and ethical considerations

The corpus uses publicly intended parliamentary materials and official metadata. Textual plenary records are openly accessible under Bundestag archival rules, while audiovisual usage follows Mediathek licensing terms for educational, cultural, and parliamentary use with source attribution and without misleading modification.

Archival materials that require additional permissions are referenced via IDs or links but are not redistributed as raw audiovisual files. The release focuses on transparency, traceability, and legal compliance and contains no private personal data.

## Citation

Please cite the archived release associated with the version you used. A Zenodo DOI should be added once the first public release is created.

Example citation format:

I. Siegert. 2026. *GerParlDia-MM: A Multimodal Diachronic Corpus of German Parliamentary Debates (1949-2025).* to appear in LREC 2026 proceedings. DOI to be added.

If you use GitHub, you can also enable citation support through the included `CITATION.cff` file.

## Recommended repository structure

```text
.
├── index.html
├── README.md
├── CITATION.cff
├── LICENSE
└── data/ or docs/ (optional)
```

## Publishing as a website

You can host this repository as a static website:

- **GitHub Pages:** deploy from the repository root or `/docs`
- **GitLab Pages:** deploy as a static site via Pages

Since your repository already contains an `index.html`, it can be used directly as the landing page.

## Release workflow recommendation

For scientific use, the recommended workflow is:

1. Maintain the living project page in this Git repository.
2. Create versioned releases in Git.
3. Archive each release via Zenodo.
4. Cite the specific Zenodo DOI in papers.
5. Link the website to the Zenodo concept DOI and/or version DOI.

## Contact

Please add the responsible contact person or corresponding authors here.

## License

The data used in this project are not publicly available due to privacy and
ethical considerations. Access to the data may be granted upon reasonable
request to the authors.
