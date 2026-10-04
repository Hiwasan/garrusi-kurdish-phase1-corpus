# Known issues

This document records the anomalies present in version 1.0.0 of the
corpus. They are preserved as-is because they reflect the source data.

## Duplicated utterance ID in S22

Speaker S22 contains two rows with the utterance ID `S22_090`. Both are
genuine utterances (one long, one short) that were assigned the same ID
in the source files. Users should treat `utt_id` as non-unique for S22
unless they also check the `garrusi` column.

## Placeholder row in S03

Speaker S03 had a source row with an ID containing only dashes. It was
skipped during corpus construction and does not appear in the published
data.

## Timestamps removed

Version 1.0.0 does not include `start_s` or `end_s` columns. Timestamps
were part of the source data but were removed from the published corpus
because the audio is not distributed here and the timestamps contained
inconsistencies. A future version may reintroduce them.

## Persian translation removed

The source transcripts included a Persian translation column. It was
removed from version 1.0.0 due to script and encoding considerations.
A future version may reintroduce it.

## Reporting issues

If you find a problem not listed here, please open an issue on the
repository.