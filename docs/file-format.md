# File format

Each speaker is provided as a separate UTF-8, tab-separated file named
`S01.tsv`, `S02.tsv`, … `S30.tsv`. Speaker identities are pseudonymized;
the mapping between speaker codes and individuals is not published.

## Columns

| Column | Description |
|---|---|
| `speaker` | Speaker ID (`S01` … `S30`). |
| `utt_id` | Utterance ID, unique within a speaker (`S01_001`, `S01_002`, …). |
| `section` | Either `Questionnaire` (elicited responses) or `Story Narration` (narrative retellings). |
| `elicitation_item` | For questionnaire rows, the stimulus item (e.g. `P1: To bury`). Empty for narration rows. |
| `prompt` | The interviewer's question in Garrusi, repeated for each response to that prompt. Empty when the row has no prompt. |
| `garrusi` | The Garrusi Kurdish utterance as transcribed by the fieldworker. |
| `english` | English translation of the utterance. |

## Notes

- All files are UTF-8 encoded, tab-separated, with a header row.
- Blank cells indicate missing information, not empty strings.
- Utterance IDs are not globally unique across speakers; use the
  combination of `speaker` and `utt_id` as a compound key.
- The transcriptions retain the orthographic conventions of the original
  fieldwork. See `docs/orthography.md`.