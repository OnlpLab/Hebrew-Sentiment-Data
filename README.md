# Hebrew-Sentiment-Data
A cleaned version of the Hebrew Sentiment data set published by Amram, A., Ben-David, A., and Tsarfaty, R. (2018). Representations and Architectures in Neural Sentiment Analysis for Morphologically Rich Languages: A Case Study from Modern Hebrew. In: Proceedings of The 27th International Conference on Computational Linguistics (COLING 2018) Santa Fe, NM, (pp. 2242-2252).
Original dataset can be found under the omilab [Github][1].  

Since reported the data to be leaking (shared material between test and train) we provide a cleaned up version, with a new split of train-dev-test, instead of the original train-test. We provide in this repository both the new clean data and both the deduping code.


Data and cleaning process information:  
| Data set | Original Set sizes | Deduped Set sizes| Comment |
| -------- | -------------- |-------------- |-------------- |
| Train    | 9220           |
| Dev      | 1026           |
| Test     | 2561           |

Original Set sizes  
Train: 9220  
Dev (Originally didn't exist and was part of the train): 1026  
Test: 2561  
Total original size:  12807  

----
duplication within the sets:  

| Data set | Leakage percentage |
| -------- | -------------- |
| Train    | 24.6%          |
| Dev      | 3.8%           |
| Test     | 7.53%          |

Leakage between data sets: 

| Data set | Leakage |
| -------- | -------------- |
| Test - Train    | 1120 (12%)          |
| Test + Dev - Train      | 1685 (16.22%)          |


[1]:  https://github.com/omilab/Neural-Sentiment-Analyzer-for-Modern-Hebrew
