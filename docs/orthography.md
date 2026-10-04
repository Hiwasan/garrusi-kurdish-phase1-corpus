# Orthography

The Garrusi transcriptions use a Latin-based orthography. This note
describes the character set and records open questions.

## Character set

The corpus uses the standard Latin letters plus the following:

| Character | Unicode | Notes |
|---|---|---|
| `ç` | U+00E7 | Voiceless postalveolar affricate |
| `ê` | U+00EA | Long mid front vowel |
| `î` | U+00EE | Long high front vowel |
| `û` | U+00FB | Long high back vowel |
| `ü` | U+00FC | High front rounded vowel |
| `ş` | U+015F | Voiceless postalveolar fricative |
| `ř` | U+0159 | See "Open questions" below |
| `ł` | U+0142 | See "Open questions" below |
| `’` | U+2019 | See "Open questions" below |
| `ˀ` | U+02C0 | See "Open questions" below |
| `“ ”` | U+201C U+201D | Quotation marks within utterances |
| `…` | U+2026 | Ellipsis, used for unfinished utterances |

## Open questions

The following orthographic questions are carried forward from the
fieldwork and are pending confirmation with the transcription team.
They do not affect the usability of version 1.0.0, but users should be
aware of them.

1. **`ř`** appears systematically in verb forms such as `biřîyaye`,
   `kutuřilî`, `diřilî`. Its phonetic value needs to be confirmed
   (candidate values include a trill and a retroflex flap).

2. **`ł`** appears in a small number of tokens such as `minał`
   ("child"). It may be a distinct velar lateral or a typographic
   variant of `l`. It is preserved as written in the source.

3. **`’` (U+2019) and `ˀ` (U+02C0)** both appear as glottal-stop-like
   marks. Whether they distinguish different sounds or are variants of
   the same mark is an open question. Both are preserved in the corpus
   as written.

## Normalization

The corpus is stored in Unicode NFC. No normalization beyond NFC has
been applied to the transcriptions; the characters above are preserved
exactly as they appear in the source documents.