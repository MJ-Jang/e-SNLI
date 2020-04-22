# News

**`!`** New work on e-SNLI: [Make Up Your Mind! Adversarial Generation of Inconsistent Natural Language Explanations](https://arxiv.org/abs/1910.03065). Accepted as a short paper at ACL, 2020.

**`!`** New dataset of visual textual entailment with natural language explanations taken from e-SNLI: [e-SNLI-VE-2.0: Corrected Visual-Textual Entailment with Natural Language Explanations](https://arxiv.org/abs/2004.03744). At the IEEE CVPR Workshop on Fair, Data Efficient and Trusted Computer Vision, 2020

**`!`** If are also interested in feature-based explanations besides natural language explanations, check out our new work on verifying post-hoc explanatory methods: [Can I Trust the Explainer? Verifying Post-hoc Explanatory Methods](https://arxiv.org/abs/1910.02065). At NeurIPS 2019 Workshop on Safety and Robustness in Decision Making, 2020.

# e-SNLI
There are 2 splits for the train set due to the github sie restrictions, please simply merge them.

Clarification on the two potentially confusing headers:
* Sentence1_marked_1: is the premise (Sentence2 for hypothesis) were words between star (*) were highlighted by the annotators. The annotators had to click on every word individually to highlght it. The punctuation has not been separated from the words, hence highlighting a word automatically included any punctuation near it.
* Sentence1_Highlighted_1: is the list of indices of the highlighted words, where the index starts at 0 and the organization is only done by splitting with space.

The tokanization for models was more advance and can be found in https://github.com/OanaMariaCamburu/e-SNLI/blob/master/tokenizer.sed. Our models do not make use of the highlighted words.

# Trained models
Trained models can be downloaded at:
* PredictAndExplain: https://drive.google.com/file/d/1w8UlNQ5yvZPNu4RgVkgICB6qsefkjolG/view?usp=sharing
* ExplainThenPredictAttention: https://drive.google.com/file/d/1l7dnml7mDnT72QrwZMmA7VGIsWjVpQT6/view?usp=sharing
* ExplanationsToLabels: https://drive.google.com/file/d/1_rFGlFYHSJ1xqjA2lDjzBvO5mf7INo1A/view?usp=sharing

# Dependancies
* Python 2.7
* Pytorch 0.3.1
* NLTK >= 3

# Bibtex
If you use this dataset or code in your work, please cite [our paper](https://papers.nips.cc/paper/8163-e-snli-natural-language-inference-with-natural-language-explanations.pdf):
```
@incollection{NIPS2018_8163,
title = {e-SNLI: Natural Language Inference with Natural Language Explanations},
author = {Camburu, Oana-Maria and Rockt\"{a}schel, Tim and Lukasiewicz, Thomas and Blunsom, Phil},
booktitle = {Advances in Neural Information Processing Systems 31},
editor = {S. Bengio and H. Wallach and H. Larochelle and K. Grauman and N. Cesa-Bianchi and R. Garnett},
pages = {9539--9549},
year = {2018},
publisher = {Curran Associates, Inc.},
url = {http://papers.nips.cc/paper/8163-e-snli-natural-language-inference-with-natural-language-explanations.pdf}
}
