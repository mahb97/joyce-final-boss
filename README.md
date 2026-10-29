# James Joyce as the Final Boss of NLP 

> "What can’t be coded can be decorded if an ear aye seize what no eye ere grieved for” (FW 482.34–36).

Code and data for *James Joyce as the Final Boss of NLP*, in preparation for DH2027 (University of Galway, June 2027).

## Overview 

Standard NLP pipeline components are run across a difficulty gradient of Joyce's prose: *Dubliners* 
(the tutorial level), *Ulysses* (the mid-game), and *Finnegans Wake* (the final boss). 
Each component's degradation along the gradient is measured, and its failure modes are read as diagnostics of 
the linguistic assumptions the tools encode: a single named language, stable word-hood, the existence of a lemma, 
a sentiment lexicon's referential innocence. Failure as methodology (Rettberg 2022), applied literally.

## Status

Pipelines under construction. Expect breakage; some of it is the point.

## Planned experiments

- [ ] Corpus assembly and provenance notes
- [ ] Tokenisation (spaCy, NLTK, subword/BPE): cross-tool agreement, type/token behaviour
- [ ] Stopword filtering: list coverage across the gradient
- [ ] Stemming (Porter, Snowball) and lemmatisation (spaCy, WordNet): coverage and collision rates
- [ ] POS tagging (spaCy, NLTK): cross-tagger agreement as a proxy for confidence collapse
- [ ] NER (spaCy): precision spot-checks against human annotation
- [ ] Sentiment (VADER, TextBlob): lexicon coverage and output stability
- [ ] Figures and write-up

Each experiment lives in a numbered script, writes its outputs to `results/`, and is run with fixed seeds where 
randomness is involved.

## Corpora and copyright

*Dubliners* and *Ulysses* are taken from Project Gutenberg. *Finnegans Wake* has been in the public domain in 
the EU since 2012 but remains in copyright in the United States, so the full text is **not** committed to this 
repository; scripts expect a local copy at `data/` and the exact source and preprocessing are documented 
in `data/README.md`. Derived statistics and counts are included in full.

## Structure (planned)

```
data/        corpora and provenance notes (Wake text not committed; see above)
pipelines/   numbered experiment scripts
results/     metrics, tables, intermediate outputs
figures/     plots used in the paper
```

## AI disclosure

[Placeholder: statement consistent with the DH2027 submission's generative AI disclosure.]

## Citation

[Placeholder: citation and DOI to follow upon submission.]

## Licence

Code under MIT. Text, figures, and derived data under CC BY 4.0.
