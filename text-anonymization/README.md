# Manually annotated Wikipedia summaries

A dataset of 553 Wikipedia summaries, manually annotated for text anonymization, along with the annotation guidelines.

Out of all the texts, 20 were annotated by 2 annotators instead of 1. Each annotation is assigned the following:

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


##Citation

See our paper describing the dataset:

Anthi Papadopoulou, Pierre Lison, Lilja Øvrelid and Ildikó Pilán (2022), "[Bootstrapping Text Anonymization Models with Distant Supervision](https://aclanthology.org/2022.lrec-1.476/)", *In Proceedings of the Thirteenth Language Resources and Evaluation Conference, pages 4477–4487, Marseille, France. European Language Resources Association.*

```bibtex
@inproceedings{papadopoulou-etal-2022-bootstrapping,
    title = "Bootstrapping Text Anonymization Models with Distant Supervision",
    author = "Papadopoulou, Anthi  and
      Lison, Pierre  and
      {\O}vrelid, Lilja  and
      Pil{\'a}n, Ildik{\'o}",
    booktitle = "Proceedings of the Thirteenth Language Resources and Evaluation Conference",
    month = jun,
    year = "2022",
    address = "Marseille, France",
    publisher = "European Language Resources Association",
    url = "https://aclanthology.org/2022.lrec-1.476",
    pages = "4477--4487",
    abstract = "We propose a novel method to bootstrap text anonymization models based on distant supervision. Instead of requiring manually labeled training data, the approach relies on a knowledge graph expressing the background information assumed to be publicly available about various individuals. This knowledge graph is employed to automatically annotate text documents including personal data about a subset of those individuals. More precisely, the method determines which text spans ought to be masked in order to guarantee k-anonymity, assuming an adversary with access to both the text documents and the background information expressed in the knowledge graph. The resulting collection of labeled documents is then used as training data to fine-tune a pre-trained language model for text anonymization. We illustrate this approach using a knowledge graph extracted from Wikidata and short biographical texts from Wikipedia. Evaluation results with a RoBERTa-based model and a manually annotated collection of 553 summaries showcase the potential of the approach, but also unveil a number of issues that may arise if the knowledge graph is noisy or incomplete. The results also illustrate that, contrary to most sequence labeling problems, the text anonymization task may admit several alternative solutions.",
}
