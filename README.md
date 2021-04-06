# Hebrew-Sentiment-Data
A cleaned version of the Hebrew Sentiment data set published by Amram, A., Ben-David, A., and Tsarfaty, R. (2018).[1]
Original dataset can be found under the omilab [Github][1].  

Since we discovered that there was a data leakage (shared material between test and train) we provide a cleaned version without duplications and with removal of text that is almost identical. (for example 2 samples that say "I love you!" and "I love you!!" considerd identical), with a new split of train-dev-test, instead of the original train-test. We provide in this repository both the new clean data and both the full deduping code.


### Data and cleaning process information :
| Data set | Original Set sizes | Deduped Set sizes - Token     | Deduped Set sizes - Morph | Comment    |
| -------- | --------------     |--------------------           |--------------             |------------|
| Train    | 9220               |   5926                        |5932                       |            |
| Dev      | 1026               |   846                         |847                        | Originally didn't exist and was part of the train|
| Test     | 2561               |   1695                        |1696                       |             |
 
###   Duplication within the sets:  

| Data set | Leakage percentage |
| -------- | -------------- |
| Train    | 24.6%          |
| Dev      | 3.8%           |
| Test     | 7.53%          |

#### Leakage between data sets: 

| Data set | Leakage |
| -------- | -------------- |
| Test - Train    | 1120 (12%)          |
| Test + Dev - Train      | 1685 (16.22%)          |


[1]:  https://github.com/omilab/Neural-Sentiment-Analyzer-for-Modern-Hebrew
[1]  Representations and Architectures in Neural Sentiment Analysis for Morphologically Rich Languages: A Case Study from Modern Hebrew. In: Proceedings of The 27th International Conference on Computational Linguistics (COLING 2018) Santa Fe, NM, (pp. 2242-2252).
