## Natural Language Toolkit for Indic Languages (iNLTK)

[![Gitter](https://badges.gitter.im/inltk/community.svg)](https://gitter.im/inltk/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![Downloads](https://pepy.tech/badge/inltk)](https://pepy.tech/project/inltk)

iNLTK aims to provide out of the box support for various NLP tasks 
that an application developer might need for Indic languages. Paper for iNLTK library has been accepted at EMNLP-2020's NLP-OSS workshop. Here's the [preprint for the paper](https://arxiv.org/abs/2009.12534)


### Documentation

Checkout detailed docs along with Installation instructions
 at https://inltk.readthedocs.io


### Supported languages

| Language | Code <code-of-language> |
|:--------:|:----:|
|   Hindi  |  hi  |
|  Punjabi |  pa  |
| Gujarati |  gu  |
|  Kannada |  kn  |
| Malayalam |  ml  |
|   Oriya   |  or  |
|  Marathi |  mr  |
|  Bengali |  bn  |
|   Tamil  |  ta  |
|   Urdu  |  ur  |
|  Nepali  |  ne  |
| Sanskrit |  sa  |
|   English  |  en  |

#### Repositories containing models used in iNLTK

|  Language |                            Repository                            |                                                                                     Dataset used for Language modeling                                                                                     | Perplexity of ULMFiT LM<br>(on validation set) | Perplexity of TransformerXL LM<br>(on validation set) |                                                                                                                                                                                    Dataset used for Classification                                                                                                                                                                                    |  Classification:<br> Test set Accuracy  |     Classification: <br>Test set MCC    | Classification: Notebook<br>for Reproducibility                                                                                                                                                                                                                                                                                                                                                                                                  |                                                                                ULMFiT Embeddings visualization                                                                               |                                                                                  TransformerXL Embeddings visualization                                                                                  |
|:---------:|:----------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------:|:-----------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------:|:---------------------------------------:|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|   Hindi   |     [NLP for Hindi](https://github.com/goru001/nlp-for-hindi)    | [Hindi Wikipedia Articles - 172k](https://www.kaggle.com/disisbig/hindi-wikipedia-articles-172k)<br><br><br>[Hindi Wikipedia Articles - 55k](https://www.kaggle.com/disisbig/hindi-wikipedia-articles-55k) |             34.06<br><br><br>35.87             |                 26.09<br><br><br>34.78                | [BBC News Articles](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)<br><br><br>[IIT Patna Movie Reviews](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)<br><br><br>[IIT Patna Product Reviews](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets) | 78.75<br><br><br>57.74<br><br><br>75.71 | 71.61<br><br><br>37.23<br><br><br>59.76 | [Notebook](https://github.com/goru001/nlp-for-hindi/blob/master/classification-benchmarks/Hindi_Classification_Model_BBC_Articles.ipynb)<br><br><br>[Notebook](https://github.com/goru001/nlp-for-hindi/blob/master/classification-benchmarks/Hindi_Classification_Model_IITP%2BMovie.ipynb)<br><br><br>[Notebook](https://github.com/goru001/nlp-for-hindi/blob/master/classification-benchmarks/Hindi_Classification_Model_IITP_Product.ipynb) |   [Hindi Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-hindi/master/language-model/embedding_projector_config_30k.json)  |    [Hindi Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-hindi/master/language-model/embedding_projector_config_transformerxl.json)   |
|  Bengali  |   [NLP for Bengali](https://github.com/goru001/nlp-for-bengali)  |                                                          [Bengali Wikipedia Articles](https://www.kaggle.com/disisbig/bengali-wikipedia-articles)                                                          |                      41.2                      |                          39.3                         |                                                                                                                               [Bengali News Articles (Soham Articles)](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)                                                                                                                              |                  90.71                  |                  87.92                  | [Notebook](https://github.com/goru001/nlp-for-bengali/blob/master/classification/Bengali_Classification_Model.ipynb)                                                                                                                                                                                                                                                                                                                             |   [Bengali Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-bengali/master/language-model/embedding_projector_config.json)  |   [Bengali Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-bengali/master/language-model/embedding_projector_transformer_config.json)  |
|  Gujarati |  [NLP for Gujarati](https://github.com/goru001/nlp-for-gujarati) |                                                         [Gujarati Wikipedia Articles](https://www.kaggle.com/disisbig/gujarati-wikipedia-articles)                                                         |                      34.12                     |                         28.12                         |                                                                                                                                 [iNLTK Headlines Corpus - Gujarati](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)                                                                                                                                 |                  91.05                  |                  86.09                  | [Notebook](https://github.com/goru001/nlp-for-gujarati/blob/master/classification/Gujarati_Classification_Model.ipynb)                                                                                                                                                                                                                                                                                                                           |  [Gujarati Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-gujarati/master/language-model/embedding_projector_config.json) |  [Gujarati Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-gujarati/master/language-model/embedding_projector_transformer_config.json) |
| Malayalam | [NLP for Malayalam](https://github.com/goru001/nlp-for-malyalam) |                                                        [Malayalam Wikipedia Articles](https://www.kaggle.com/disisbig/malayalam-wikipedia-articles)                                                        |                      26.39                     |                         25.79                         |                                                                                                                                 [iNLTK Headlines Corpus - Malayalam](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)                                                                                                                                |                  95.56                  |                  93.29                  | [Notebook](https://github.com/goru001/nlp-for-malyalam/blob/master/classification/Malyalam_Classification_Model.ipynb)                                                                                                                                                                                                                                                                                                                           | [Malayalam Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-malyalam/master/language-model/embedding_projector_config.json) | [Malayalam Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-malyalam/master/language-model/embedding_projector_transformer_config.json) |
|  Marathi  |   [NLP for Marathi](https://github.com/goru001/nlp-for-marathi)  |                                                          [Marathi Wikipedia Articles](https://www.kaggle.com/disisbig/marathi-wikipedia-articles)                                                          |                       18                       |                         17.42                         |                                                                                                                                  [iNLTK Headlines Corpus - Marathi](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)                                                                                                                                 |                  92.40                  |                  85.23                  | [Notebook](https://github.com/goru001/nlp-for-marathi/blob/master/classification/Marathi_Classification_Model.ipynb)                                                                                                                                                                                                                                                                                                                             |   [Marathi Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-marathi/master/language-model/embedding_projector_config.json)  |   [Marathi Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-marathi/master/language-model/embedding_projector_transformer_config.json)  |
|   Tamil   |     [NLP for Tamil](https://github.com/goru001/nlp-for-tamil)    |                                                            [Tamil Wikipedia Articles](https://www.kaggle.com/disisbig/tamil-wikipedia-articles)                                                            |                      19.80                     |                         17.22                         |                                                                                                                                   [iNLTK Headlines Corpus - Tamil](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)                                                                                                                                  |                  95.22                  |                  92.70                  | [Notebook](https://github.com/goru001/nlp-for-tamil/blob/master/classification/Tamil_Classifier.ipynb)                                                                                                                                                                                                                                                                                                                                           |     [Tamil Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-tamil/master/language-model/embedding_projector_config.json)    |     [Tamil Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-tamil/master/language-model/embedding_projector_transformer_config.json)    |
|  Punjabi  |   [NLP for Punjabi](https://github.com/goru001/nlp-for-punjabi)  |                                                          [Punjabi Wikipedia Articles](https://www.kaggle.com/disisbig/punjabi-wikipedia-articles)                                                          |                      24.40                     |                         14.03                         |                                                                                                                      [IndicNLP News Article Classification Dataset - Punjabi](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#indicnlp-news-article-classification-dataset)                                                                                                                     |                  97.12                  |                  96.17                  | [Notebook](https://github.com/goru001/nlp-for-punjabi/blob/master/classification/Panjabi_Classification_Model.ipynb)                                                                                                                                                                                                                                                                                                                             |   [Punjabi Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-punjabi/master/language-model/embedding_projector_config.json)  |   [Punjabi Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-punjabi/master/language-model/embedding_projector_transformer_config.json)  |
|  Kannada  |   [NLP for Kannada](https://github.com/goru001/nlp-for-kannada)  |                                                          [Kannada Wikipedia Articles](https://www.kaggle.com/disisbig/kannada-wikipedia-articles)                                                          |                      70.10                     |                         61.97                         |                                                                                                                      [IndicNLP News Article Classification Dataset - Kannada](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#indicnlp-news-article-classification-dataset)                                                                                                                     |                  98.87                  |                  98.30                  | [Notebook](https://github.com/goru001/nlp-for-kannada/blob/master/classification/Kannada_Classification_Model.ipynb)                                                                                                                                                                                                                                                                                                                             |   [Kannada Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-kannada/master/language-model/embedding_projector_config.json)  |   [Kannada Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-kannada/master/language-model/embedding_projector_transformer_config.json)  |
|   Oriya   |     [NLP for Oriya](https://github.com/goru001/nlp-for-odia)     |                                                             [Oriya Wikipedia Articles](https://www.kaggle.com/disisbig/odia-wikipedia-articles)                                                            |                      26.57                     |                         26.81                         |                                                                                                                       [IndicNLP News Article Classification Dataset - Oriya](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#indicnlp-news-article-classification-dataset)                                                                                                                      |                  98.83                  |                  98.44                  | [Notebook](https://github.com/goru001/nlp-for-odia/blob/master/classification/Oriya_Classification_Model.ipynb)                                                                                                                                                                                                                                                                                                                                  |     [Oriya Embeddings Projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-odia/master/language-model/embedding_projector_config.json)     |     [Oriya Embeddings Projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-odia/master/language-model/embedding_projector_transformer_config.json)     |
|  Sanskrit |  [NLP for Sanskrit](https://github.com/goru001/nlp-for-sanskrit) |                                                         [Sanskrit Wikipedia Articles](https://www.kaggle.com/disisbig/sanskrit-wikipedia-articles)                                                         |                       ~6                       |                           ~3                          |                                                                                                                                                          [Sanskrit Shlokas Dataset](https://www.kaggle.com/disisbig/sanskrit-shlokas-dataset)                                                                                                                                                         |             84.3 (valid set)            |                                         |                                                                                                                                                                                                                                                                                                                                                                                                                                                  |  [Sanskrit Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-sanskrit/master/language-model/embedding_projector_config.json) |  [Sanskrit Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-sanskrit/master/language-model/embedding_projector_transformer_config.json) |
|   Nepali  |    [NLP for Nepali](https://github.com/goru001/nlp-for-nepali)   |                                                           [Nepali Wikipedia Articles](https://www.kaggle.com/disisbig/nepali-wikipedia-articles)                                                           |                      31.5                      |                          29.3                         |                                                                                                                                                               [Nepali News Dataset](https://www.kaggle.com/disisbig/nepali-news-dataset)                                                                                                                                                              |             98.5 (valid set)            |                                         |                                                                                                                                                                                                                                                                                                                                                                                                                                                  |    [Nepali Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-nepali/master/language-model/embedding_projector_config.json)   |    [Nepali Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-nepali/master/language-model/embedding_projector_transformer_config.json)   |
|    Urdu   |    [NLP for Urdu](https://github.com/anuragshas/nlp-for-urdu)    |                                                             [Urdu Wikipedia Articles](https://www.kaggle.com/disisbig/urdu-wikipedia-articles)                                                             |                      13.19                     |                         12.55                         |                                                                                                                                                                 [Urdu News Dataset](https://www.kaggle.com/disisbig/urdu-news-dataset)                                                                                                                                                                |            95.28 (valid set)            |                                         |                                                                                                                                                                                                                                                                                                                                                                                                                                                  |    [Urdu Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/anuragshas/nlp-for-urdu/master/language-model/embedding_projector_config.json)    |    [Urdu Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/anuragshas/nlp-for-urdu/master/language-model/embedding_projector_transformer_config.json)    |

Note: English model has been directly taken from [fast.ai](https://github.com/fastai/fastai)

#### Effect of using Transfer Learning + Paraphrases from iNLTK

|  Language |                            Repository                            |                                                       Dataset used for Classification                                                      | Results on using<br>complete training set | Percentage Decrease <br>in Training set size | Results on using<br>reduced training set<br>without Paraphrases | Results on using<br>reduced training set<br>with Paraphrases |
|:---------:|:----------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------:|:--------------------------------------------:|:------------------------------------------------------------:|:---------------------------------------------------------:|
|   Hindi   |     [NLP for Hindi](https://github.com/goru001/nlp-for-hindi)    |         [IIT Patna Movie Reviews](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)        |     Accuracy: 57.74<br><br>MCC: 37.23     |               80% (2480 -> 496)              |               Accuracy: 47.74<br><br>MCC: 20.50              |             Accuracy: 56.13<br><br>MCC: 34.39             |
|  Bengali  |   [NLP for Bengali](https://github.com/goru001/nlp-for-bengali)  | [Bengali News Articles (Soham Articles)](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets) |     Accuracy: 90.71<br><br>MCC: 87.92     |              99% (11284 -> 112)              |               Accuracy: 69.88<br><br>MCC: 61.56              |             Accuracy: 74.06<br><br>MCC: 65.08             |
|  Gujarati |  [NLP for Gujarati](https://github.com/goru001/nlp-for-gujarati) |    [iNLTK Headlines Corpus - Gujarati](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)   |     Accuracy: 91.05<br><br>MCC: 86.09     |               90% (5269 -> 526)              |               Accuracy: 80.88<br><br>MCC: 70.18              |             Accuracy: 81.03<br><br>MCC: 70.44             |
| Malayalam | [NLP for Malayalam](https://github.com/goru001/nlp-for-malyalam) |   [iNLTK Headlines Corpus - Malayalam](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)   |     Accuracy: 95.56<br><br>MCC: 93.29     |               90% (5036 -> 503)              |               Accuracy: 82.38<br><br>MCC: 73.47              |             Accuracy: 84.29<br><br>MCC: 76.36             |
|  Marathi  |   [NLP for Marathi](https://github.com/goru001/nlp-for-marathi)  |    [iNLTK Headlines Corpus - Marathi](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)    |     Accuracy: 92.40<br><br>MCC: 85.23     |               95% (9672 -> 483)              |               Accuracy: 84.13<br><br>MCC: 68.59              |             Accuracy: 84.55<br><br>MCC: 69.11             |
|   Tamil   |     [NLP for Tamil](https://github.com/goru001/nlp-for-tamil)    |     [iNLTK Headlines Corpus - Tamil](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)     |     Accuracy: 95.22<br><br>MCC: 92.70     |               95% (5346 -> 267)              |               Accuracy: 86.25<br><br>MCC: 79.42              |             Accuracy: 89.84<br><br>MCC: 84.63             |

For more details around implementation or to reproduce results, checkout respective repositories. 

### Contributing

##### Add a new language support

If you would like to add support for language of your own choice to iNLTK,
 please start with checking/raising a issue [here](https://github.com/goru001/inltk/issues)
 
Please checkout the steps I'd [mentioned here for Telugu](https://github.com/goru001/inltk/issues/1)
to begin with. They should be almost similar for other languages as well.

##### Improving models/using models for your own research

If you would like to take iNLTK's models and refine them with your own 
dataset or build your own custom models on top of it, please check out the 
repositories in the above table for the language of your choice. The repositories above 
contain links to datasets, pretrained models, classifiers and all of the code for that.

##### Add new functionality

If you wish for a particular functionality in iNLTK - Start by checking/raising a issue [here](https://github.com/goru001/inltk/issues)


### What's next


#### ..and being worked upon
`Shout out if you want to help :)`

* Add [Telugu](https://github.com/goru001/inltk/issues/1) 
and [Maithili](https://github.com/goru001/inltk/issues/10) support


#### ..and NOT being worked upon

`Shout out if you want to lead :)`

* Add NER support for all languages
* Add Textual Entailment support for all languages
* Work on a [unified model for all the languages](https://github.com/goru001/inltk/issues/14)
* [POS support](https://github.com/goru001/inltk/issues/13) in iNLTK
* Add translations - to and from languages in iNLTK + English



### iNLTK's Appreciation

* [By Jeremy Howard on Twitter](https://twitter.com/jeremyphoward/status/1111318198891110402)
* [By Sebastian Ruder on Twitter](https://twitter.com/seb_ruder/status/1207074241830674438)
* [By Vincent Boucher](https://www.linkedin.com/feed/update/urn:li:activity:6517137647310241792/), [By Philip Vollet](https://www.linkedin.com/posts/philipvollet_machinelearning-datascience-nlp-activity-6698220942910468096-phA-), [By Steve Nouri](https://www.linkedin.com/posts/stevenouri_india-artificialintelligence-technology-activity-6698815315498868736-vYmZ) on [LinkedIn](https://www.linkedin.com/search/results/content/?keywords=inltk)
* [By Kanimozhi](https://www.linkedin.com/feed/update/urn:li:activity:6517277916030701568), [By Soham](https://www.linkedin.com/feed/update/urn:li:activity:6513084638955696128), [By Imaad](https://www.linkedin.com/feed/update/urn:li:activity:6536258026687557632/) on [LinkedIn](https://www.linkedin.com/search/results/content/?keywords=inltk)
* iNLTK was [trending on GitHub](https://github.motakasoft.com/trending/ranking/monthly/?d=2019-05-01&l=python&page=2) in May 2019


### Citation

If you use this library in your research, please consider citing citing:

```latex
@misc{arora2020inltk,
      title={iNLTK: Natural Language Toolkit for Indic Languages}, 
      author={Gaurav Arora},
      year={2020},
      eprint={2009.12534},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
