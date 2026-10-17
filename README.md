# Garrusi Kurdish Corpus, Phase 1

[!\[DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23121203.svg)](https://doi.org/10.5281/zenodo.23121203)

**Version 1.0.1** | Concept DOI (all versions): [10.5281/zenodo.23121203](https://doi.org/10.5281/zenodo.23121203) | Licence: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (full text in [LICENSE](LICENSE))

**Authors:** Hiwa Asadpour and Masoumeh Zarei (both authors contributed equally).

Copyright © 2026 Hiwa Asadpour and Masoumeh Zarei.

A text corpus of elicited Mehraban Garrusi (Southern Kurdish) speech with English translation: **30 speakers, 8,866 utterances**.

\---

## 1\. Contents

```
data/          S01.tsv ... S30.tsv   one file per speaker
docs/          file-format.md, orthography.md, known-issues.md
README.md  LICENSE  CITATION.cff
```

## 2\. Data format

Each file is UTF-8 plain text, tab-separated, with one header row and one utterance per row.

|Column|Content|
|-|-|
|`speaker`|Speaker ID (S01 to S30). IDs are pseudonyms.|
|`utt\_id`|Utterance ID: speaker ID plus the running number from the source transcript (e.g. `S01\_001`). Numbering follows the source, so gaps can occur. See *Known issues* for one duplicated ID.|
|`section`|`Questionnaire` or `Story Narration`.|
|`elicitation\_item`|The target verb of the questionnaire item (P1 to P20, e.g. "P1: To bury"). Empty in `Story Narration`.|
|`prompt`|The question put to the speaker in Garrusi, for questionnaire responses.|
|`garrusi`|Transcription of the speaker's utterance (Latin-based orthography, see below).|
|`english`|English translation.|

## 3\. Transcription and translation conventions

* **Orthography.** A Latin-based transcription with the characters `ç ê î û ü ş ř`. Details are in `docs/orthography.md`.
* **English translations.** `\[= ... ]` gives a paraphrase of the preceding literal translation (for example a passive paraphrase of an impersonal active).
* Utterances are kept as spoken, including false starts and repetitions.

## 4\. Background and data collection

### The research program

The corpus belongs to the research program *Passive and Relative Clauses in Iranian and non-Iranian Languages: Experimental and Empirical Approach*, initiated and led by Hiwa Asadpour.

The programme began as Asadpour's postdoctoral project on passive and relative clauses in Mukri Kurdish, Kurmanji Kurdish and Persian, with extensions to Azeri Turkish and Armenian. Local researchers in Iran then joined the initiative to extend the work to further Iranian and non-Iranian languages, including Laki Kurdish, Nayini, Kahangi, Kilani, Sistani Persian, Azeri Turkish and Garrusi Kurdish. Garrusi was added when Masoumeh Zarei joined the programme. The programme began in 2019, and the collaboration on Garrusi dates from 2021. The consortium that collected the Phase 1 data was unfunded.

### The Garrusi fieldwork

Garrusi has two subdialects, Mehraban and Bijar. This corpus documents Mehraban Garrusi, the variety spoken by all 30 participants.

This corpus is the result of fieldwork conducted by Masoumeh Zarei in February and March 2021. The research design, methodology, research questions, elicitation protocol, questionnaire and stimulus materials were developed by Hiwa Asadpour, who also provided guidance on data collection, transcription, translation and formatting. Masoumeh Zarei conducted the fieldwork on this basis, interviewing 30 native speakers in Qohurd-e Olya (Upper Qohurd), a village in Mehraban-e Sofla Rural District, Kabudarahang County, Hamadan Province. The name Qohurd historically goes back to the word Gaukhaud /gaw xwad/ and means "cow eater". In the travelogue of Bird (1891), the village of Gaukhaud is mentioned as the border separating Persian-speaking and Kurdish-speaking lands (Bird 1891, 176-177; Zarei 2025, 5-6).

In the first part of each interview, Masoumeh Zarei showed the participants 20 event-driven pictures, each accompanied by three questions. First, they were asked to describe what they observed in each picture. Then they were asked two questions, one about an animate entity and the other about an inanimate entity, both of which were the subject of actions performed by an agent. In the second part, she played the Pear Story film for the participants and asked them to re-narrate it. A total of 780 minutes (13 hours) of voice recordings were made during the questionnaire and the narrative task. She then transcribed the recordings using the Kurdish Roman alphabet and translated them into Persian and English, and clause-level annotation was carried out as part of the work on the data.

This release contains the Garrusi transcription and the English translation only. The audio recordings, the Persian translation and the annotation are not part of it (see section 6).

Phase 1 has two parts:

1. **Questionnaire.** Picture-based elicitation with a visual questionnaire built on Montag and MacDonald (2013), covering 20 target verbs, with standardised prompts.
2. **Story narration.** Retelling of a story, based on the Pear Story materials (Chafe 1975/1980).

The stimulus pictures are not included in this repository.

## 5\. Roles and contributions

Hiwa Asadpour initiated the program and developed the research design, methodology and research questions, as well as the elicitation protocol, questionnaire and stimulus materials. He provided guidance and feedback on data collection, transcription, translation and formatting, corrected typographical, duplication and matching errors, checked consistency, converted the data to the release format, and prepared the files and documentation for publication.

Masoumeh Zarei conducted the fieldwork and interviewed the participants, transcribed the recordings, translated them into Persian and English and pseudonymised the transcripts under the guidance and feedback from Hiwa Asadpour.

Both authors contributed equally to the corpus.

## 6\. Not included

* **Audio recordings.** Not published.
* is release and may be added in a later version.
* **Annotation.** Clause-level annotation was carried out as part of the work on the data. It is not part of this release.
* **Speaker identities.** The key linking speaker codes to individuals is held privately and is not distributed.

## 7\. Ethics, consent and privacy

Participants took part voluntarily and were not paid. Their consent to be recorded was documented at the start of each recording. Masoumeh Zarei, who obtained the participants' consent during the fieldwork, confirms that the consent and ethics arrangements permit the publication of the name of the village and other location details.

Speakers appear only under the codes S01 to S30. Speakers' names and personal details are not published.

Although speakers' names are not published, the corpus may contain information that, alone or combined with other information, could help to identify a speaker. Please do not attempt to identify the speakers, and follow the applicable standards of research ethics and data protection in your own use of the corpus.

**Removal requests.** If you are a speaker, or a relative of one, and want material removed, contact one of the authors (see section 11). We will review the request and, where appropriate, remove or restrict access to the material in the repository and request corresponding action from Zenodo. We cannot guarantee removal from copies that have already been downloaded or archived by others.

## 8\. Licence and reuse

This corpus is released under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). The full text is in the [LICENSE](LICENSE) file. You are free to use, share and adapt it for any purpose, including commercial, provided you give appropriate credit as described under *How to cite*.

Each author may use the corpus in their own research. Publications that use this corpus should cite this release. Authorship of any later publication depends on the contributions made to that publication.

Users who build on the elicitation protocol or research questions of the program are asked to acknowledge the program and Hiwa Asadpour's contribution to its protocols and research questions.

## 9\. How to cite

> Asadpour, H., \& Zarei, M. (2026). \*Garrusi Kurdish Corpus, Phase 1\* \[Data set]. Zenodo. https://doi.org/10.5281/zenodo.23121203

Authors are listed alphabetically; both contributed equally. For the exact release used, cite the version-specific DOI shown on the Zenodo record. The DOI above (all versions) may be used to refer to the corpus in general.

Please also cite the related publications where relevant:

* *Passive Constructions in Garrusi Kurdish* (2026). https://doi.org/10.11647/obp.0516.05
* *Corpus and Experimental Analysis of Passive Structures in Garrusi Kurdish.* Languages, 2026, 11, 63. https://doi.org/10.3390/languages11040063

Other sources cited in this README:

* Bird, I. (1891). *Journeys in Persia and Kurdistan: including a summer in the upper Karun region and a visit to the Nestorian rayahs*, volume 2. New York: Cambridge University Press.
* Zarei, M. (2025). *Typology of Argument Structure in the Complex Predicates of Garrusi Kurdish* \[PhD dissertation]. Allameh Tabataba'i University, Tehran.
* Montag, J. L., \& MacDonald, M. C. (2013). Visual salience modulates structure choice in relative clause production. *Language and Speech*, 57(2), 163-180. https://doi.org/10.1177/0023830913495656
* Chafe, W. L. (1975). The pear film. University of California. https://www.youtube.com/watch?v=bRNSTxTpG7U (accessed 02 October 2026).

## 10\. Known issues

* One source row in speaker S03 contained only placeholder dashes and was omitted.
* Speaker S22 has two utterances with the same ID (S22\_090). Both are genuine; users should treat `utt\_id` as non-unique for S22.
* The corpus is a transcription of spoken language and may contain transcription and translation errors. Corrections are welcome as issues or pull requests.

## 11\. Contact

* Hiwa Asadpour, asadpourhiwa@gmail.com
* Masoumeh Zarei, zareimasoumeh26@gmail.com

For questions and removal requests, contact either author.

## 12\. Acknowledgements

We thank the 30 speakers for their participation.

## 13\. Changelog

* **v1.0.1** `17.10.2026`: published the corpus as the original Word documents (one per speaker) instead of the tab-separated files used in v1.0.0; added the description of the fieldwork and the authors line; revised the roles section; stated the reasons for omitting audio and annotation; corrected the license text, the citation file and the removal-request wording. Version DOI: [10.5281/zenodo.23435349](https://doi.org/10.5281/zenodo.23435349).
* **v1.0** (3 October 2026): first release.

