# Garrusi Kurdish Corpus, Phase 1
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23121203.svg)](https://doi.org/10.5281/zenodo.23121203)

**Version 1.0** | DOI: [10.5281/zenodo.23121203](https://doi.org/10.5281/zenodo.23121203) | Licence: [CC BY 4.0](LICENSE)

A text corpus of elicited Garrusi (Southern Kurdish) speech with English translation: **30 speakers, 8,866 utterances**.

---

## 1. Contents

```
data/          S01.tsv ... S30.tsv   one file per speaker
docs/          file-format.md, orthography.md, known-issues.md
README.md  LICENSE  CITATION.cff
```

## 2. Data format

Each file is UTF-8 plain text, tab-separated, with one header row and one utterance per row.

| Column | Content |
|---|---|
| `speaker` | Speaker ID (S01 to S30). IDs are pseudonyms. |
| `utt_id` | Unique utterance ID: speaker ID plus the running number from the source transcript (e.g. `S01_001`). Numbering follows the source, so gaps can occur. |
| `section` | `Questionnaire` or `Story Narration`. |
| `elicitation_item` | The target verb of the questionnaire item (P1 to P20, e.g. "P1: To bury"). Empty in `Story Narration`. |
| `prompt` | The question put to the speaker in Garrusi, for questionnaire responses. |
| `garrusi` | Transcription of the speaker's utterance (Latin-based orthography, see below). |
| `english` | English translation. |

## 3. Transcription and translation conventions

- **Orthography.** A Latin-based transcription with the characters `ç ê î û ü ş ř`. Details are in `docs/orthography.md`.
- **English translations.** `[= ... ]` gives a paraphrase of the preceding literal translation (for example a passive paraphrase of an impersonal active).
- Utterances are kept as spoken, including false starts and repetitions.

## 4. Background and data collection

The corpus belongs to the research programme *Passive and Relative Clauses in Iranian and non-Iranian Languages: Experimental and Empirical Approach*, initiated and led by Hiwa Asadpour.

The program began as Asadpour's postdoctoral project on passive and relative clauses in Mukri Kurdish, Kurmanji Kurdish and Persian, with extensions to Azeri Turkish and Armenian. Local researchers in Iran then joined the initiative to extend the work to further Iranian and non-Iranian languages, including Laki Kurdish, Nayini, Kahangi, Kilani, Sistani Persian, Azeri Turkish, and Garrusi Kurdish. Garrusi is spoken across a wide area and exhibits internal variation; the variety documented in this release is one of several. Users comparing it with other Garrusi material should treat the varieties as distinct. The current released Garrusi was added later, when Masoumeh Zarei joined the program.

Key dates: the program began in 2019; the collaboration on Garrusi released here dates from 2021.

Phase 1 consists of approximately 13 hours of recordings with 30 native speakers of Garrusi, and has two parts:

1. **Questionnaire.** Picture-based elicitation with a visual questionnaire built on Montag and MacDonald (2013), covering 20 target verbs, with standardized prompts.
2. **Story narration.** Retelling of a story, based on the Pear Story materials (Chafe 1975/1980).

The stimulus pictures are not included in this repository.

The project was unfunded.

## 5. Roles and contributions

Roles follow the CRediT taxonomy (https://credit.niso.org/).

| Role | Hiwa Asadpour | Masoumeh Zarei |
|---|---|---|
| Conceptualisation, research questions and research design | yes | |
| Methodology (elicitation protocol, questionnaire and stimulus design, transcription and translation conventions) | yes | |
| Investigation (participant contact, fieldwork, recording) | | yes |
| Data creation (transcription, translation into English and Persian, initial annotation) | guidance and amendments | main work |
| Validation (checking of transcriptions and translations, quality control) | yes | |
| Data curation (format conversion, pseudonymisation, preparation for publication) | yes | |
| Documentation and repository | yes | |

## 6. Not included

- **Audio recordings.** Not published.
- **Timestamps.** The source transcripts contain start times, which are not part of this release because the audio is not published.
- **Persian translations.** The source transcripts also contain Persian translations, which are not part of v1.0. They may be added in a later version.
- **Speaker identities.** The key linking codes to individuals is held privately and is not distributed.

## 7. Ethics, consent and privacy

Participants gave consent to be recorded, which was documented at the start of each recording.

Speakers appear only under the codes S01 to S30. Names and personal details are not published. 

Please do not attempt to identify the speakers. Users are expected to follow the usual standards of research ethics and data protection in their own use of the corpus.

**Removal requests.** If you are a speaker, or a relative of one, and want material removed, contact `asadpourhiwa@gmail.com`. We will remove it from the repository and publish a corrected version on Zenodo.

## 8. License and reuse

This corpus is released under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](LICENSE). You are free to use, share, and adapt it for any purpose, including commercial, provided you give appropriate credit as described under *How to cite*.

Each author may use the corpus in their own research. Publications that use this corpus should cite this release. Authorship of any later publication depends on the contributions made to that publication.

Users who build on the elicitation protocol or research questions of the program are asked to acknowledge the program and Hiwa Asadpour's contribution to its protocols and research questions.

## 9. How to cite

> Asadpour, H., & Zarei, M. (2026). *Garrusi Kurdish Corpus, Phase 1* (Version 1.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.23121203

Please also cite the related publications where relevant:

- *Passive Constructions in Garrusi Kurdish* (2026). https://doi.org/10.11647/obp.0516.05
- *Corpus and Experimental Analysis of Passive Structures in Garrusi Kurdish.* Languages, 2026, 11, 63. https://doi.org/10.3390/languages11040063

Stimulus sources:

- Montag, J. L., & MacDonald, M. C. (2013). Visual salience modulates structure choice in relative clause production. *Language and Speech*, 57(2), 163-180. https://doi.org/10.1177/0023830913495656
- Chafe, W. L. (1975). The pear film. University of California. Available online: https://www.youtube.com/watch?v=bRNSTxTpG7U (accessed on 02 October 2026).

## 10. Known issues

- One source row in speaker S03 contained only placeholder dashes and was omitted.
- Speaker S22 has two utterances with the same ID (S22_090). Both are genuine; users should treat utt_id as non-unique for S22.
- The corpus is a transcription of spoken language and may contain transcription and translation errors. Corrections are welcome as issues or pull requests.

## 11. Contact

Hiwa Asadpour, asadpourhiwa@gmail.com for questions and removal requests

## 12. Acknowledgements

We thank the 30 speakers for their participation.

## 13. Changelog

- **v1.0** `03.10.2026`: first release.
