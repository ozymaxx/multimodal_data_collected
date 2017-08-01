# Data collected in video retrieval studies
This repository contains data corpora of sketched symbols and texts transcribed from participants' speech in the studies outlined [here](https://ozymaxx.github.io/blog/2017/07/31/insan-merkezli-tasarim1/).

Note that the natural language corpus is in Turkish.

## Directory structure
* **sketched_symbols**: Each directory contains sketched symbols of a class. Each class directory has two sub-directories:
  * **image**: Image version of sketched symbols
  * **sketch**: Sketched symbols in *Points in table* format. Check [this](https://github.com/ozymaxx/sketchfe) out for further description of the format.
  Note that each symbol in both directories has the same file-name. 
* **speech_nlp**: This directory contains phrases with their class labels. Naming conventions of the files inside this directory is presented below.
  * **testphrases_libname.txt**: Phrases used for testing of a machine learning algorithm. *libname* indicates the library to use on the file (fb->[FastText](https://github.com/facebookresearch/fastText), libshort->[libshorttext](https://www.csie.ntu.edu.tw/~cjlin/libshorttext/), our->architectures that I implemented myself)
  * **trainphrases_libname.txt**: Phrases used for training of a machine learning algorithm. *libname* indicates the library to use on the file (fb->[FastText](https://github.com/facebookresearch/fastText), libshort->[libshorttext](https://www.csie.ntu.edu.tw/~cjlin/libshorttext/), our->architectures that I implemented myself)
  * **valphrases_libname.txt**: Phrases used for validation during hyperparameter search of a machine learning algorithm. *libname* indicates the library to use on the file (fb->[FastText](https://github.com/facebookresearch/fastText), libshort->[libshorttext](https://www.csie.ntu.edu.tw/~cjlin/libshorttext/), our->architectures that I implemented myself)
  * **trainvalphrases_libname.txt**: If you don't perform any hyperparameter search, just use this file for training. Training and validation sets are merged in this file. *libname* indicates the library to use on the file (fb->[FastText](https://github.com/facebookresearch/fastText), libshort->[libshorttext](https://www.csie.ntu.edu.tw/~cjlin/libshorttext/), our->architectures that I implemented myself)
  
## See Also
Codes for the analysis of the data: [https://github.com/ozymaxx/multimodal_collection_analysis](https://github.com/ozymaxx/multimodal_collection_analysis)

## Credits
Ozan Can Altıok - [Koç University Intelligent User Interfaces Laboratory](http://iui.ku.edu.tr) - oaltiok15 at ku dot edu dot tr
