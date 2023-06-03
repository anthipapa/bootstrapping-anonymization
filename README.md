A dataset of 553 summeries, manually annotated for text anonymization (text-anonymization), and further enriched with replacement options for each PII span (wiki-replace).


## Citation

See our papers describing both datasets:

# text-anonymization

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
```

# wiki-replace

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
```
