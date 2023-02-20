# Replacement choices in Text Sanitization

A enriched dataset of 553 Wikipedia summaries, manually annotated for replacement options for text sanitization, along with the annotation guidelines. Presented in "Generation of Replacement Options in Text Sanitization".

Out of all the texts, 22 were annotated by more than one annotators. Each annotation is assigned the following:

| Name | Description |
| --- | --- |
| **entity_type** | Semantic category for the span (e.g. *LOC*, *ORG*) |
| **entity_mention_id** | ID for the entity mention |
| **start_offset** | the character offset where the span starts |
| **end_offset** | the character offset where the span ends|
| **span_text** | the text of the span |
| **edit_type** | *check/insert/correct* as an action taken by the annotator |
| **identifier_type** | whether the span is a *DIRECT* or a *QUASI identifier* (masked spans), or *NO_MASK* |
| **entity_id** | which entity mention ID the entity relates to as far as meaning is concerned |
| **generalizations** | list of possible hierarchical replacements for the span |
| **generalization_selection** | which replacement was chosen by the annotator |
| **generalized_text** | the resulting text after replacements were chosen |
