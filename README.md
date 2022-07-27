# Manually annotated Wikipedia summaries

A dataset of 553 Wikipedia summaries, manually annotated for text anonymization, along with the annotation guidelines. Used for evaluation in the paper "Bootstrapping Text Anonymization Models with Distant Supervision".

Out of all the texts, 20 were annotated by 2 annotators instead of 1. Each annotation is assigned the following:

| Name | Description |
| --- | --- |
| **entity_type** | Semantic category for the span (e.g. *LOC*, *ORG*) |
| **entity_mention_id** | ID for the mention |
| **start_offset** | the character offset where the span starts |
| **end_offset** | the character offset where the span ends|
| **span_text** | the text of the span |
| **edit_type** | check/insert/correct as an action taken by the annotator |
| **identifier_type** | whether the span is a *DIRECT* or a *QUASI identifier* (and thus masked), or *NO_MASK* |
| **entity_id** | which entity mention ID the entity related to as far as meaning is concerned |
