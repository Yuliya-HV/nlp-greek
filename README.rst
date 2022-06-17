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

Greek language is spoken by majority of population in two countries.

======================================================== 
Country / ISO Language code
======================================================== 
.. image:: https://img.shields.io/badge/Cyprus-cy-green           


.. image:: https://img.shields.io/badge/Greek-gr-green            
========================================================



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
Greek text requires accents and diacritics removal. Some new Tokenizers include this step but earliest editions doesn not.
https://legacy.cltk.org/en/latest/greek.html


Lemmatization
~~~~~~~~~~~~~~~~~~~

`Spacy lemmatizer (trainable lemmatizer) <https://spacy.io/api/lemmatizer>`_

`JohnSnowLabs Greek lemmatizer <https://nlp.johnsnowlabs.com/2020/05/05/lemma_el.html>`_

`CLTK Greek lemmatiter <https://legacy.cltk.org/en/latest/greek.html#lemmatization>`_


Tokenization
~~~~~~~~~~~~~~~~~~~

Depends on a sutiation we might need different corpus tokenization. Sources below include general tokenizers for word, sentence, paragraph tokenization.


NLTK
^^^^^^^^^^^^^^^^^^^^^^^^^^^
`NLTK tokenizer module <https://www.nltk.org/api/nltk.tokenize.html>`_

Spacy
^^^^^^^^^^^^^^^^^^^^^^^^^^^
`Spacy Tokenizer <https://spacy.io/api/tokenizer>`_
Also available a pipeline component for Greek language **senter** for Sentence segmentation.


Other 
~~~~~~~~~~~~~~~~~~~
Spacy offers other helpful components:
morphologizer, dependency parser, attribute ruler.


NLP tasks
----------

Named Entity Recognition
~~~~~~~~~~~~~~~~~~~

=============  =================================================  ===============================================================
Source         Supported labels                                   Link
=============  =================================================  ===============================================================
Spacy          EVENT, GPE, LOC, ORG, PERSON, PRODUCT              `Spacy models <https://spacy.io/models/el>`_


Spark NLP


Stanza


AUEB           LOC, ORG, PERSON,                                  `gr-nlp-toolkit <https://github.com/nlpaueb/gr-nlp-toolkit>`_
                                                                  transformer-based
=============  =================================================  ===============================================================


Translation
~~~~~~~~~~~~~~~~~~~

=============  =================================================  =============================================
Package        Details                                            Link
=============  =================================================  =============================================
Spark NLP      Multilingual (wrapped from Hugging Face)


Transformers   Multilingual 
=============  =================================================  =============================================


Transformers model
-------------------

BERT model pretrained on Greek corpus only.

**bert-base-greek-uncased-v1**

`Greek BERT <https://github.com/nlpaueb/greek-bert>`_


Other
------

Proper nouns
~~~~~~~~~~~~
`List of 144,000 Classical Greek proper nouns <https://github.com/cltk/greek_proper_names_cltk>`_


Ancient Greek
~~~~~~~~~~~~~~
`Some handy stuff for Ancient Greek <https://legacy.cltk.org/en/latest/greek.html>`_

