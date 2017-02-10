# DHd2017-semsearch-cuneiform 

This project contains the accompanying code for the following publication:

```
@InProceedings{daxenbergerEtAl:2017:DHd,
  author    = {Johannes Daxenberger and Susanne Görke and Darjush Siahdohoni and Iryna Gurevych and Doris Prechel},
  title     = {Semantische Suche in Ausgestorbenen Sprachen: Eine Fallstudie für das Hethitische},
  booktitle = {Extended Abstract at DHd 2017},
  month     = feb,
  year      = {2017},
  address   = {Bern, Switzerland}
}
```

> **Abstract:** We present a semantic search engine for translations of Cuneiform documents. The motivation for this work is to make the contant of the documents more accessible for reseachers outside the domain of Ancient Assyriology. We use state-of-the-art lexical-semantic methods to process a collection of Hittite documents. A smale-scale user survey proves the usefullness and inituitive usage of the resulting web-based search engine.

A demo of the tool is available [here](http://semsearch.ukp.informatik.tu-darmstadt.de).

This work has been carried out in collabroation with the Department for [Ancient Philology](http://www.ao.altertumswissenschaften.uni-mainz.de) at the Johannes Gutenberg-Universität Mainz.

Contact person: Johannes Daxenberger, daxenberger@ukp.informatik.tu-darmstadt.de

https://www.ukp.tu-darmstadt.de/

https://www.tu-darmstadt.de/


Don't hesitate to send us an e-mail or report an issue, if something is broken (and it shouldn't be) or if you have further questions.

> This repository contains experimental software and is published for the sole purpose of giving additional background details on the respective publication. 


## Requirements

* Java 7 or higher
* Maven
* Tested under Windows 7

## Installation

 * You need a Uby database to run the experiments
 * All other dependencies should be handeled via Maven.

## Running the experiments

The main class is:
```
RunPipeline
```

### Parameter description

* `OUTPUT_DESTINATION`
  * where to write the output
* `INPUT_LOCATION`
  * location of the ODT-Files
* `ALTERNATIVE_WRITING_DATASET` 
  * location of the alternative writings dictionary (opt.)
* `HYPERNYMS_DATASET`
  * location of the hypernyms dictionary (opt.)
* `INPUT_FILE_LANGUAGE`
  * language of the files to be processed
  * Supported Languages: German (de), English (en), French (fr), Italian (it)
* `STOP_WORD_LIST_LOCATION`
  * stopword list location
* `TRANSLITERATION_VERSION`
  * The version of the transliteration. Usually double dash "--" indicates the master transliteration. But some files contain "-het", or "-akk"

For Uby:

* `DB_URL`
* `DB_DRIVER`
* `DB_DRIVER_NAME`
* `DB_USERNAME`
* `DB_PASSWORD`

