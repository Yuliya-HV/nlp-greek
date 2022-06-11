NLP for Greek language
==========

This repo is an aggregation of sources for Greek language to tackle varios Natural Language Processing/Understanding/Generation needs.

**Contents**

.. contents::
  :local:
  :depth: 3
  :backlinks: none



The language and countries
---------------------------

Greek language is used in varios countries.

=========== ==========================================================
Country     ISO Language code
=========== ==========================================================
🇨🇾          .. image:: https://img.shields.io/badge/Cyprus-el-green


🇬🇷          .. image:: https://img.shields.io/badge/Greek-el-green
=========== ==========================================================



Greek Tree Bank
---------
Morphological and syntatic annotations of Greek corpus. This Greek UD source used by many other pretrained open-source components. 

**Manually annotated**: lemmas, dependencies, POS, features.

**Genres**: news, wiki, spoken

**Souces**: public domain, wikinews articles, European Parlament sessions texts.

**Corpus size**: 2521 sentences/ 61.673 tokens.


https://universaldependencies.org/treebanks/el_gdt/index.html



Pipeline Components
---------

Accentuation and diacritics
~~~~~~~~~~~~~~~~~~~
Greek text requires accents removal.


Lemmatization
~~~~~~~~~~~~~~~~~~~

https://legacy.cltk.org/en/latest/greek.html


https://spacy.io/models/el

https://nlp.johnsnowlabs.com/2020/05/05/lemma_el.html


Tokenization
~~~~~~~~~~~~~~~~~~~

Word
^^^^^^^^^^^^^^^^^^^^^^^^^^^

Sentence
^^^^^^^^^^^^^^^^^^^^^^^^^^^

Paragraph
^^^^^^^^^^^^^^^^^^^^^^^^^^^

 tok2vec, morphologizer, parser, lemmatizer (trainable_lemmatizer), senter, ner, attribute_ruler.


NLP tasks
----------

Named Entity Recognition
~~~~~~~~~~~~~~~~~~~

=============  =================================================  ===============================================================
Source         Supported labels                                   Link
=============  =================================================  ===============================================================
Spacy          EVENT, GPE, LOC, ORG, PERSON, PRODUCT              `Spacy models <https://spacy.io/models/el>`_


Stanza


Spark NLP


AUEB           LOC, ORG, PERSON,                                  `gr-nlp-toolkit <https://github.com/nlpaueb/gr-nlp-toolkit>`_
                                                                  transformer-based
=============  =================================================  ===============================================================


Translation
~~~~~~~~~~~~~~~~~~~

=============  =================================================  =============================================
Package        Details                                            Link
=============  =================================================  =============================================
Spark NLP      Multilingual (wrapped from Hugging Face)


Transformers   
=============  =================================================  =============================================


General model
-------------

BERT model pretrained on Greek corpus 

..code: bert-base-greek-uncased-v1

`Greek BERT <https://github.com/nlpaueb/greek-bert>` _
