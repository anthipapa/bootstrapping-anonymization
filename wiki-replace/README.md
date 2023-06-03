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



##Citation

See our paper describing the dataset:

Annika Willoch Olstad, Anthi Papadopoulou, and Pierre Lison. 2023. "[Generation of Replacement Options in Text Sanitization](https://aclanthology.org/2023.nodalida-1.30/)". *In Proceedings of the 24th Nordic Conference on Computational Linguistics (NoDaLiDa), pages 292–300, Tórshavn, Faroe Islands. University of Tartu Library.*


```bibtex
@inproceedings{olstad-etal-2023-generation,
    title = "Generation of Replacement Options in Text Sanitization",
    author = "Olstad, Annika Willoch  and
      Papadopoulou, Anthi  and
      Lison, Pierre",
    booktitle = "Proceedings of the 24th Nordic Conference on Computational Linguistics (NoDaLiDa)",
    month = may,
    year = "2023",
    address = "T{\'o}rshavn, Faroe Islands",
    publisher = "University of Tartu Library",
    url = "https://aclanthology.org/2023.nodalida-1.30",
    pages = "292--300",
    abstract = "The purpose of text sanitization is to edit text documents to mask text spans that may directly or indirectly reveal personal information. An important problem in text sanitization is to find less specific, yet still informative replacements for each text span to mask. We present an approach to generate possible replacements using a combination of heuristic rules and an ontology derived from Wikidata. Those replacement options are hierarchically structured and cover various types of personal identifiers. Using this approach, we extend a recently released text sanitization dataset with manually selected replacements. The outcome of this data collection shows that the approach is able to suggest appropriate replacement options for most text spans.",
}
