# Deep Transfer Learning Baselines for Sentiment Analysis in Russian

This repository contains the fine-tuned Multilingual Bidirectional Encoder Representations from Transformers (M-BERT) (Devlin et al., 2019) and two versions of Multilingual Universal Sentence Encoder (M-USE) (Yang et al., 2019) for sentiment classification in Russian. Initially we were supposed to outline transfer learning baselines, but eventually, we achieved state-of-the-art results on the majority of datasets.

| System  | RuReviews | RuReviews | Kaggle Russian News Dataset | LINIS Crowd | RuTweetCorp | 
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| Previous SOTA | 75.45% | **78.50%** | 70.00% | 37.29% | 75.95% | 
| M-BERT-Base-FiT | **77.31%** | 72.44% | 71.36% | 42.73% | **87.38%** |
| M-BERT-Base-SNPT-FiT | – | 75.13% | – | – | – |
| M-USE-CNN-FiT | 76.63% | 70.88% | **72.66%** | 56.34% | 85.53% |
| M-USE-Trans-FiT | 76.94% | 73.37% | 66.85% | **56.95%** | 87.12% |

SOTA approaches for RuReviews, RuSentiment, Kaggle Russian News Dataset, and RuTweetCorp were described in papers (Smetanin and Komarov, 2019), (Baymurzina et al., 2019), (Shalkarbayuli et al., 2018), 857 and (Rubtsova, 2018), consequently. The SOTA approach for LINIS Crowd was implemented based on the paper (Koltsova et al., 2016).

## Sentiment Datasets in Russian
Despite the fact that Russian is one of the most common languages in the World Wide Web, generally it is not as well-resourced as the English language, especially in the field of sentiment analysis. Even though many studies aim at sentiment classification, only few of them makes their datasets publicly available for the research community. To the best of our knowledge, there are only five public datasets for sentiment analysis in Russian. The statistics for each dataset can be found in the table below.

| Dataset  | Classes | Average lengths | Max lengths | Train Samples | Test Samples | Overall Samples | Download Link |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| RuReviews (Smetanin and Komarov, 2019)| 3 | 130.0693 | 1007 | n/a | n/a | 90000 | [Github page](https://github.com/sismetanin/rureviews) |
| RuSentiment (Rogers et al., 2018)| 5 | 82.0279 | 800 | 28218 | 2967 | 31185 | [Project page](http://text-machine.cs.uml.edu/projects/rusentiment) |
| Kaggle Russian News Dataset (Kaggle, 2017)| 3 | 3911.8501 | 381498 | n/a | n/a | 8263 | [Kaggle page](https://www.kaggle.com/c/sentiment-analysis-in-russian) |
| LINIS Crowd (Koltsova et al., 2016)| 5  |  n/a  |  n/a  |  n/a  |  n/a  |  n/a  | [Project page](http://linis-crowd.org) |
| RuTweetCorp (Rubtsova, 2013)| 3 | 89.1725 | 189 | n/a | n/a | 334836 | [Project page](http://study.mokoron.com) |


## Fine-Tuned Models
To download fine-tuned models for Russian, please follow the link [https://yadi.sk/d/Xp5vLG_5xCQL-Q](https://yadi.sk/d/Xp5vLG_5xCQL-Q).
### RuReviews
* M-BERT-Base-FiT-RuReviews – Multilingual BERT<sub>Base</sub> fine-tuned on RuReviews.
* M-USE-CNN-FiT-RuReviews – Multilingual USE<sub>CNN</sub> fine-tuned on RuReviews.
* M-USE-Trans-FiT-RuReviews – Multilingual USE<sub>Trans</sub> fine-tuned on RuReviews.
### RuSentiment
* M-BERT-Base-FiT-RuSentiment  – Multilingual BERT<sub>Base</sub> with futher pre-training on posts from social networks fine-tuned on RuSentiment.
* M-BERT-Base-SNPT-FiT-RuSentiment – Multilingual BERT<sub>Base</sub> fine-tuned on RuSentiment.
* M-USE-CNN-FiT-RuSentiment – Multilingual USE<sub>CNN</sub> fine-tuned on RuSentiment.
* M-USE-Trans-FiT-RuSentiment – Multilingual USE<sub>Trans</sub> fine-tuned on RuSentiment.
### Kaggle Russian News Dataset
* M-BERT-Base-FiT-KSDRN – Multilingual BERT<sub>Base</sub> fine-tuned on Kaggle Russian News Dataset.
* M-USE-CNN-FiT-KSDRN – Multilingual USE<sub>CNN</sub> fine-tuned on Kaggle Russian News Dataset.
* M-USE-Trans-FiT-KSDRN – Multilingual USE<sub>Trans</sub> fine-tuned on Kaggle Russian News Dataset.
### LINIS Crowd
* M-BERT-Base-FiT-LINIS – Multilingual BERT<sub>Base</sub> fine-tuned on LINIS Crowd.
* M-USE-CNN-FiT-LINIS – Multilingual USE<sub>CNN</sub> fine-tuned on LINIS Crowd.
* M-USE-Trans-FiT-LINIS – Multilingual USE<sub>Trans</sub> fine-tuned on LINIS Crowd.
### RuTweetCorp
* M-BERT-Base-FiT-RuTweetCorp – Multilingual BERT<sub>Base</sub> fine-tuned on RuTweetCorp.
* M-USE-CNN-FiT-RuTweetCorp – Multilingual USE<sub>CNN</sub> fine-tuned on RuTweetCorp.
* M-USE-Trans-FiT-RuTweetCorp – Multilingual USE<sub>Trans</sub> fine-tuned on RuTweetCorp.

## References
1. Anna Rogers, Alexey Romanov, Anna Rumshisky, Svitlana Volkova, Mikhail Gronas, and Alex Gribov. 2018. RuSentiment: An enriched sentiment analysis dataset for social media in Russian. In Proceedings of the 27th International Conference on Computational Linguistics, pages 755–763, Santa Fe, New Mexico, USA. Association for Computational Linguistics.
2. Kaggle. 2017. Sentiment analysis in Russian — Kaggle.
3. Sergey Smetanin and Michail Komarov. 2019. Sentiment analysis of product reviews in Russian using convolutional neural networks. In 2019 IEEE 1174 21st Conference on Business Informatics (CBI), volume 01, pages 482–486.
4. Jacob Devlin, Ming-Wei Chang, Kenton Lee, and 950 Kristina Toutanova. 2019. BERT: Pre-training of 951 deep bidirectional transformers for language understanding. In Proceedings of the 2019 Conference of the North American Chapter of the Association 953 for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers), pages 4171–4186, Minneapolis, Minnesota. Association for Computational Linguistics.
5. Olessia Koltsova, Svetlana Alexeeva, and Sergei Kolcov. 2016. An opinion word lexicon and a training dataset for Russian sentiment analysis of social media. Computational Linguistics and Intellectual Technologies. Papers from the Annual International Conference Dialogue 2016, pages 227–287.
6. Yinfei Yang, Daniel Cer, Amin Ahmad, Mandy Guo, Jax Law, Noah Constant, Gustavo Herna ́ndez A ́brego,SteveYuan,ChrisTar,Yun-HsuanSung, Brian Strope, and Ray Kurzweil. 2019a. Multilingual universal sentence encoder for semantic retrieval. CoRR, abs/1907.04307.
7. Yuliya Rubtsova. 2013. A method for development and analysis of short text corpus for the review classification task. Proceedings of conferences Digital Libraries: Advanced Methods and Technologies, Digital Collections (RCDL’2013), pages 269–275.


## Documentation and How to report bugs
* TensorFlow documentation: [https://www.tensorflow.org/api_docs](https://www.tensorflow.org/api_docs).
* Scikit-learn documentation: [http://scikit-learn.org/stable/documentation.html](http://scikit-learn.org/stable/documentation.html). 
* BERT repository: [https://github.com/google-research/bert](https://github.com/google-research/bert). 
* If you find any issues, please open a bug here on GitHub.

## License
See [LICENSE](LICENSE.txt).
